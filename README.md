# Second Shift — secondshift.cc

Landing page for Second Shift. Static site, no build step: `index.html` is the whole thing.

## How it deploys
Connected to Vercel. Anything merged to `main` goes live automatically.
Every pull request gets its own preview URL from Vercel — check it there before merging.

## Making changes
1. Branch off `main`
2. Edit `index.html` (copy, links, sections — it's all inline)
3. Open a PR, look at the Vercel preview link, merge

The booking link appears three times — search for `calendly.com`.

## Domain
Vercel → project → Settings → Domains → add `secondshift.cc` and `www.secondshift.cc`.
Then add the two DNS records Vercel shows you at the registrar:

- `A`     `@`    `76.76.21.21`
- `CNAME` `www`  `cname.vercel-dns.com`

SSL is automatic once DNS resolves.
