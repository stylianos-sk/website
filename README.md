# Website

Personal website of Stylianos Sarantellis Komninellis.

## Theme

This site uses the [Hugo Split theme](https://themes.gohugo.io/themes/hugo-split-theme/), the source and instructions of which can be found [here](https://github.com/escalate/hugo-split-theme). It is configured as a Hugo theme using a git submodule roughly according to the [Hugo Quick start guide](https://gohugo.io/getting-started/quick-start/#explanation-of-commands).

## Hosting & Deployment

The site is hosted by [GitHub pages](https://pages.github.com/) and is available by default at https://stylianos-sk.github.io/website/. It is now also available at https://stylianos.sk.

There is a [`hugo.yaml`](./.github/workflows/hugo.yaml) [GitHub actions workflow](https://docs.github.com/en/actions/concepts/workflows-and-actions/workflows) inspired by https://github.com/actions/starter-workflows/blob/main/pages/hugo.yml located in the [`.github/workflows/`](./.github/workflows) directory in this repository which builds this hugo site on an Ubuntu machine and deploys it to GitHub pages.

The GitHub pages hosting and deployment settings are configured in https://github.com/stylianos-sk/website/settings/pages .

## TODOs

- [ ] Customise the site
- [ ] Add a favicon
- [ ] Deploy to a custom domain

