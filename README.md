# ACCESS Hive Forum discourse theme

## Installation

### Installing and enabling theme

1.  Navigate to the Discourse [theme settings page](https://forum.access-hive.org.au/admin/customize/themes).
2.  Click the "Install" button on the bottom left
3.  Select "From a git repository" in the left menu
4.  Paste this git repository's URL in the "Repository containing theme" field.
5.  Click "Install"
6.  To set as the default for all users, check "Theme is enabled by default" and save.

### CodeBlock theme component fix

This theme contains the CodeBlock component. It requires a small change to site settings to install and function properly.

1.  Head [here](https://forum.access-hive.org.au/admin/site_settings/)
2.  Search for `theme_authorized_extensions`
3.  Add `css` to the list of authorized extensions

See [here](https://meta.discourse.org/t/codeblock-theme-picker/146396/25) for more info.

### Search block component setup

To set up text for the search component:

1.  Navigate [here](https://forum.access-hive.org.au/admin/customize/components)
2.  Search for `Search banner`
3.  Add text for `search_banner.headline`
4.  Add text for `search_banner.subhead`

## Usage

### Colours

Most page colours are defined in the theme's colourscheme in `about.json`.

There are a few manually overriden colours defined in `common/colour_definitions.scss`.

Category colours can be defined as below:

1.  Navigate to the home page [category list view](https://forum.access-hive.org.au/categories).
2.  Click on the category you want to edit - for example [ACCESS-NRI Releases](https://forum.access-hive.org.au/c/access-nri-releases/75).
3.  Click the edit icon (wrench) in the top right corner to take you to the [category settings page](https://forum.access-hive.org.au/c/access-nri-releases/edit/general).
4.  Select the desired color and click "Save Category" at the bottom of the page.

### Changing forum logo

The forum logo can be changed [here](https://forum.access-hive.org.au/admin/site_settings/category/branding).

### Forum caching issue

Occasionally there may be an issue where the new theme isn't displayed properly due to your browser retaining the old theme in its cache. To solve this, hold down the shift key while clicking the refresh button at the same time to clear the cache and refresh the page.

## Development

Install pre-commit hooks: `pre-commit install`.

Run pre-commit checks/formatters on all files: `pre-commit run --all-files`.

Pre-commit pipeline configuration located in `.pre-commit-config.yaml`.
