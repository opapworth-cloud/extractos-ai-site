# ExtractOS DNS cutover to GitHub Pages

Current status, June 16, 2026:

- The ExtractOS site is deployed at https://opapworth-cloud.github.io/extractos-ai-site/
- The live extractos.ai domain still points to GoDaddy parking.
- Current DNS nameservers: ns27.domaincontrol.com, ns28.domaincontrol.com
- Current A records: 15.197.148.33, 3.33.130.190

To make extractos.ai show the new site, update DNS in GoDaddy:

A records for @:

- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

CNAME for www:

- opapworth-cloud.github.io

After DNS propagates, add the custom domain back in GitHub Pages:

- Repository: https://github.com/opapworth-cloud/extractos-ai-site
- Pages custom domain: extractos.ai
- Enforce HTTPS once GitHub finishes certificate provisioning.
