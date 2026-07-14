# Andrea Giovannetti — Academic Website

Personal academic website of **Dr Andrea Giovannetti** (quantitative criminology, economics, network science, and countering violent extremism).

- **Live site:** https://andrea-giovannetti.github.io/site
- **Built with:** [Jekyll](https://jekyllrb.com/) on a customised fork of the [al-folio](https://github.com/alshedivat/al-folio) academic theme.
- **Deployed via:** GitHub Actions (see [.github/workflows/deploy.yml](.github/workflows/deploy.yml)) to GitHub Pages on every push to `main`/`master`.

## Where things live

- Site config and feature flags: [_config.yml](_config.yml)
- Landing page / bio: [_pages/about.md](_pages/about.md)
- Publications (BibTeX, rendered by jekyll-scholar): [_bibliography/papers.bib](_bibliography/papers.bib)
- Research and policy projects: [_projects/](_projects)
- Other pages (projects, policy, media, PhD hiring, CV, teaching): [_pages/](_pages)
- Custom styles: [assets/css/main.scss](assets/css/main.scss) and [_sass/](_sass)
- A full site briefing and improvement notes: [SITE_OVERVIEW.md](SITE_OVERVIEW.md)

## Local development

```bash
bundle install
bundle exec jekyll serve
```

## Credits

The underlying architecture is the open-source [al-folio](https://github.com/alshedivat/al-folio) theme (MIT licensed), adapted here with additional pages, project write-ups, and styling.
