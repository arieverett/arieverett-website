# Migration checklist
1. Unzip and open the folder in VS Code.
2. Run `python3 -m http.server 8000` and inspect http://localhost:8000 at desktop and mobile widths.
3. Review all links and contents, including writing pages and portfolio pages.
4. Make a public GitHub repository named `arieverett-website` and upload this folder (contents at the repository root).
5. Configure GitHub Pages to deploy from `main` / `(root)`. Verify the default github.io preview.
6. In repository Pages settings, add the custom domain `arieverett.com`.
7. In the authoritative DNS provider, replace *only conflicting website records* with GitHub Pages apex A records: @ 185.199.108.153, @ 185.199.109.153, @ 185.199.110.153, @ 185.199.111.153 and www CNAME arieverett.github.io. Preserve MX, TXT, DKIM, SPF and any other subdomain records (especially dailybrief.arieverett.com).
8. Wait for DNS verification, enable HTTPS, test apex and www, all internal pages, mobile layout and email/subdomains. Only then cancel Super.
