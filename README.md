# Tax Sentinel public homepage

Status: **publication authorized; GitHub Pages enabled**. Repository: https://github.com/glas-zz-sfrog/tax-sentinel-homepage. Publishing source: main, /docs. HTTPS is enforced; no custom domain is configured. Deployment success and public availability must be verified separately.

This standalone website repository contains only public-facing HTML/CSS, one approved brand image, and deployment instructions. It is not the Tax Sentinel application repository and contains no application modules, accounts, credentials, screenshots or evidence packets. There are no dependencies, scripts, forms or browser storage.

## Preview

With an existing Python installation, run from this repository:

```powershell
python -m http.server 8790 --bind 127.0.0.1 --directory docs
```

Open `http://127.0.0.1:8790/`. Stop with Ctrl+C. Do not serve the parent application directory.

## Deployment configuration and future updates

1. Confirm the GitHub owner and create a **new, empty website-only repository**, suggested name `tax-sentinel-homepage`. Use Public if appropriate for the account's GitHub Pages plan. Do not reuse any application or trading-system repository. Do not add starter files remotely.
2. Review `git ls-files`: only this README, `.gitignore`, `.gitattributes`, `docs/index.html`, `docs/styles.css`, `docs/.nojekyll`, and `docs/assets/owl.png` should be tracked. Review the actual publication content. Never copy private source, configuration, data, screenshots or credentials into this repo.
3. From this separate repository, substitute the confirmed owner below. Initial publication used the following commands (do not repeat remote creation on an existing checkout):

```powershell
git remote add origin https://github.com/glas-zz-sfrog/tax-sentinel-homepage.git
git push -u origin HEAD:main
```

4. On that repository, open **Settings → Pages**. Set **Source: Deploy from a branch**, select **main** and **/docs**, then Save. No custom Actions workflow or package installation is required. The `.nojekyll` file marks a static site.
5. Wait for GitHub's Pages deployment to succeed, verify **Enforce HTTPS**, and use the actual **Visit site** URL reported by Pages settings. Check the page, CSS and image at that HTTPS address. Check the narrow mobile layout. Do not confuse the GitHub repository URL or localhost preview with the public homepage.
6. Record and return the verified public HTTPS URL to the operator for Alpaca Connect registration. Expected project-site shape is `https://OWNER.github.io/tax-sentinel-homepage/`; this is a template, not a deployed URL or a guaranteed domain. The selected owner is glas-zz-sfrog.

After Pages is enabled, future pushes to the selected source publish changes. Obtain the applicable publishing authorization before such pushes. No OAuth callback handler belongs on this public informational site; do not replace the application's separately registered local callback with the homepage URL.

## Publication copy and boundaries

The page identifies a private, locally operated tax-analysis application, not a trading service. Synthetic analyst capabilities and broker connectivity under validation are distinguished. It makes no live-sync, production tax-readiness, global tax-clearance, Alpaca approval or endorsement claim. No contact details, legal identity, account access or public download are invented. The privacy text describes this static website, not a formal privacy policy for a future multi-user service.

The owl PNG is a public branding asset supplied for this project. All browser assets are served locally; no external font, tracker, script or form endpoint is included. The external GitHub privacy link is informational only.

## GitHub documentation

- [Publishing source settings](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [HTTPS](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https)

Use the actual Pages settings and deployment result as the authority for the final URL. Local preparation does not establish a public website or provider registration approval.
