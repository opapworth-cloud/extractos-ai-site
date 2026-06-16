# ExtractOS DNS cutover

Current status, June 16, 2026:

- The ExtractOS website repo is public at https://github.com/opapworth-cloud/extractos-ai-site
- GitHub Pages is live at https://opapworth-cloud.github.io/extractos-ai-site/
- The live `extractos.ai` web domain still points to GoDaddy parking.
- Google Workspace email is live. Do not remove Google MX, SPF, DKIM, DMARC, or verification records.
- Current DNS nameservers: ns27.domaincontrol.com, ns28.domaincontrol.com
- Current web A records: 15.197.148.33, 3.33.130.190
- Current MX records include Google's `aspmx.l.google.com` mail exchangers.

When ready to launch on `extractos.ai`, update DNS in GoDaddy.

A records for `@`:

- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

CNAME for `www`:

- opapworth-cloud.github.io

After DNS propagates, add the custom domain in GitHub Pages:

- Repository: https://github.com/opapworth-cloud/extractos-ai-site
- Pages custom domain: extractos.ai
- Enforce HTTPS once GitHub finishes certificate provisioning.

Do not touch Google Workspace MX records. Web hosting and email can coexist on the same domain.
