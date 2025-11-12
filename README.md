# Website

Personal website of Stylianos Sarantellis Komninellis.

## Theme

This site uses the [Hugo Split theme](https://themes.gohugo.io/themes/hugo-split-theme/), the source and instructions of which can be found [here](https://github.com/escalate/hugo-split-theme). It is configured as a Hugo theme using a git submodule (named `split`) roughly according to the [Hugo Quick start guide](https://gohugo.io/getting-started/quick-start/#explanation-of-commands).

## Content

To change the main text of the website, please edit the [`_index.md`](./content/_index.md) file, and other text like the contact info can be edited via the [`hugo.toml`](./hugo.toml) config file. These files, just like other files in this repository, can be edited directly using GitHub, please see the [Editing files in your repository](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files#editing-files-in-your-repository) documentation, and feel free to commit directly to the `main` branch.

## Hosting & Deployment

The site is hosted by [GitHub pages](https://pages.github.com/) and is available by default at https://stylianos-sk.github.io/website/. It is now also available at https://stylianos.sk, see the [Domain Management](#domain-management) section for more details.

There is a [`hugo.yaml`](./.github/workflows/hugo.yaml) [GitHub actions workflow](https://docs.github.com/en/actions/concepts/workflows-and-actions/workflows) inspired by https://github.com/actions/starter-workflows/blob/main/pages/hugo.yml located in the [`.github/workflows/`](./.github/workflows) directory in this repository which builds this hugo site on an Ubuntu machine and deploys it to GitHub pages.

The GitHub pages hosting and deployment settings are configured in https://github.com/stylianos-sk/website/settings/pages.

## Domain Management

The custom domain, [`stylianos.sk`](https://stylianos.sk) is configured with GitHub pages according to the [Configuring a custom domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site) documentation.

The domain is managed by the registrar [Platon](https://www.platon.net/), with the DNS configuration being accessible after logging in [here](https://setup.platon.net/?lang=en_US). The domain points to GitHub Pages' servers by pointing four `A` records and four `AAAA` records to the servers' IPs, as explained by the [Configuring an apex domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain) documentation. The DNS records for stylianos.sk can be checked by an online DNS checker, for example [here](https://www.nslookup.io/domains/stylianos.sk/dns-records/).

There is a redirect from https://www.stylianos.sk to https://stylianos.sk set up using a `CNAME` record (for `www.stylianos.sk` with the value `stylianos.sk`) as explained by [Using an apex domain for your GitHub Pages site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages#using-an-apex-domain-for-your-github-pages-site) and [Configuring an apex domain and the www subdomain variant](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain-and-the-www-subdomain-variant) guides. The DNS records for www.stylianos.sk can be seen [here](https://www.nslookup.io/domains/www.stylianos.sk/dns-records/).

HTTPS and certificate provisioning is fully managed by GitHub pages, and HTTPS is enforced for the website following the [Enforcing HTTPS for your GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/securing-your-github-pages-site-with-https#enforcing-https-for-your-github-pages-site) guide.

To prevent domain takeovers by other GitHub users, the `stylianos.sk` domain is verified for this GitHub profile (`stylianos-sk`) [here](https://github.com/settings/pages) alongside a `TXT` record for `_github-pages-challenge-stylianos-sk.stylianos.sk`, which can be seen [here](https://www.nslookup.io/domains/_github-pages-challenge-stylianos-sk.stylianos.sk/dns-records/). This is done according to the [Verifying a domain for your user site](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages#verifying-a-domain-for-your-user-site) guide.

## Copyright and License

All content in this repository and on the website apart from the theme is copyrighted by Stylianos Sarantellis Komninellis and licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/). The site theme is licensed under the [Creative Commons Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/) and so the attribution on the website to the author should be kept; please see additional information [here](https://github.com/escalate/hugo-split-theme?tab=readme-ov-file#license).

## TODOs

- [x] Customise the site
- [x] Add a favicon
- [x] Deploy to a custom domain
- [ ] Update the main text
- [ ] Fix the contact and other links
- [ ] Add the social preview image
