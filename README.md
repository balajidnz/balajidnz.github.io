# sunair.fun

The front door. A list of games; each game is its own repo.

## How the URLs work

This repo **must be named `balajidnz.github.io`** — that makes it a GitHub *user site*,
and a user site is the only kind that lends its custom domain to the others.

[Per GitHub's docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages):
if a user site has a custom domain, **every project repo on the same account is served under
that domain, at a path matching the repo name.**

So:

| repo | serves |
|---|---|
| `balajidnz.github.io` (this one, holds the `CNAME`) | `sunair.fun` |
| any game repo (**no CNAME**) | `sunair.fun/<repo-name>/` |

**Adding a game is: make a repo, turn Pages on, add an `<li>` here.** Nothing else.

Two things that bite, both learned the hard way:
**only ONE repo may hold a `CNAME`** (two and they fight over the domain), and the
**repo name IS the URL and URLs are case-sensitive** — so name repos in lowercase, or every
link you have already sent out will 404.

## Why no games are listed

Not an oversight. The first game is deployed but deliberately **unlinked**, and its markup is
kept **out of `index.html` entirely** rather than commented out — a commented-out `<a href>`
is still shipped to every visitor, and anyone opening view-source reads the URL it was
supposed to be hiding. **A comment is not a secret.**

The empty-state block in `index.html` removes itself automatically once a real game exists
(`body:has(.game) .empty`), so publishing is: add the `<li>`, add the artwork, push.

## Contact

hello@sunair.fun — a real mailbox, with SPF, DKIM and DMARC.
