---
title: README
---

This repo contains a minimal Jekyll-based portfolio for lerumolamohale.me.

To publish locally and push:

1. Create the repo (recommended name: mailalebelo.github.io)
   - On GitHub, click New repository, name it mailalebelo.github.io, set it public.

2. Locally (first time)
   - git clone git@github.com:mailalebelo/mailalebelo.github.io.git
   - cd mailalebelo.github.io
   - (create files or paste the files from this repo)
   - git add .
   - git commit -m "Initial portfolio"
   - git push -u origin main

3. In the repository Settings → Pages
   - Branch: main (root)
   - Custom domain: lerumolamohale.me
   - Wait for DNS to propagate, then check "Enforce HTTPS" when available.

DNS with Namecheap (set these records)
- For apex domain (lerumolamohale.me) add four A records:
  - Host: @  Type: A  Value: 185.199.108.153
  - Host: @  Type: A  Value: 185.199.109.153
  - Host: @  Type: A  Value: 185.199.110.153
  - Host: @  Type: A  Value: 185.199.111.153
- For www (recommended) add a CNAME:
  - Host: www  Type: CNAME  Value: mailalebelo.github.io

Propagation & HTTPS
- DNS propagation can take up to 24–48 hours (often much faster).
- After DNS resolves, go to repo Settings → Pages and enable HTTPS ("Enforce HTTPS").
- Confirm by visiting https://lerumolamohale.me

If you prefer the site hosted on a different repo name or via Vercel/Netlify, follow the host-specific instructions — I can prepare a Vercel setup if you want serverless forms or booking functions.
