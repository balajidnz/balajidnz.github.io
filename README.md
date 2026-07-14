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
| `clucolor` (**no CNAME**) | `sunair.fun/clucolor/` |

**Adding a game is: make a repo, turn Pages on, add an `<li>` here.** Nothing else.
