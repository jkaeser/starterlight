# Starterlight

A starter theme for Drupal 8 projects.

- [Configuration](#configuration)
   - [Options](#options)
   - [Local configuration overrides](#local-configuration-overrides)

## Configuration
Theme configuration is in the `config.default.json` file. You will probably be happy with most of the defaults in this file, though you should absolutely tailor these options for each theme:

```
"local": "Enter the most commonly used local environment address, e.g. 'sitename.lndo.site' for sites with Lando support."
"favicons": {
  "config": {
    "appName": "Enter the name of the site or app here",
    "appDescription": "Enter a short description of the site or app here",
    "appleStatusBarStyle": "Style for Apple status bar: 'black-translucent', 'default', or 'black'",
    "background": "Hexadecimal background color for flattened icons.",
    "theme_color": "Hexadecimal color used, for example, in Android's task switcher.",
  }
}
```

### Options
**local** (string)

Your local development environment address.

**sourcemaps** (bool)

Turn Sass sourcemaps on or off.

**sass** (obj)

An object of [node-sass configuration options](https://github.com/sass/node-sass#options).

**sassLint** (obj)

An object of [sass-lint configuration options](https://github.com/sasstools/sass-lint#configuring).

**autoprefixer** (obj)

An object of [autoprefixer configuration options](https://github.com/postcss/autoprefixer#options).

**favicons** (obj)

- **source**: The path to the image file from which the rest of the favicons will be created.
- **imgDir**: The directory the generated favicons will be placed in.
- **config**: An object of [favicons configuration options](https://github.com/itgalaxy/favicons#usage).

### Local configuration overrides
You can override the default configuration for just your local environment by creating a `config.json` file at the theme root. Copy the configuration from `config.default.json` you want to override into `config.json` and customize the values.
