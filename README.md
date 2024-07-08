# ACCESS Hive Forum discourse theme

## Installation

### CodeBlock theme component installation

This theme contains the CodeBlock component. It requires a small change to site
settings to install and function properly.

1.  Head to `your.site.com/admin/site_settings/`
2.  Search for `theme_authorized_extensions`
3.  Add `css` to that list

See [here](https://meta.discourse.org/t/codeblock-theme-picker/146396/25) for
more info.

### Search block component setup

To set up text for the search component:

1.  Navigate to: `your.site.com/admin/customize/components`
2.  Search for `Search banner`
3.  Add text for `search\_banner.headline`
4.  Add text for `search\_banner.subhead`

## Development

Install pre-commit hooks: `pre-commit install`.

Run pre-commit checks/formatters on all files: `pre-commit run --all-files`.

Pre-commit pipeline configuration located in `.pre-commit-config.yaml`.
