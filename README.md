# Personal site for Max Blumberg

This repository contains a simple GitHub Pages site (index.html + CSS).

To publish:
1. Add these files to the repository root (index.html is already present, plus `assets/styles.css`, `CNAME`).
2. Push to the default branch (main).
3. In the repository Settings → Pages, set the source to Branch: `main` and / (root) folder. Save.
4. Configure DNS at GoDaddy (see instructions below).
5. After DNS propagates, enable "Enforce HTTPS" in Pages settings.

Notes:
- Replace `assets/photo.jpg` with your actual headshot.
- Replace placeholders (email, phone, CV.pdf) with real content.

GoDaddy DNS settings to point docmaxblumberg.com to GitHub Pages (summary):
- Add A records for the apex (Host = @) to these GitHub Pages IPs (one record per IP):
  - 185.199.108.153
  - 185.199.109.153
  - 185.199.110.153
  - 185.199.111.153
- Add a CNAME for the www subdomain:
  - Type: CNAME, Host: www, Points to: docmaxblumberg.github.io
- TTL: leave default or 1 hour. DNS propagation can take minutes to 48 hours.

After DNS updates and GitHub Pages shows the custom domain, enable "Enforce HTTPS".

Replace content suggestions:
- Prominently show: "Certified California Qualified Medical Examiner (QME)" near your name.
- Include a short line explaining what QME means and services you offer related to worker's compensation and IMEs.
