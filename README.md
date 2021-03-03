# syzygy-callysto, A theme for hugo

This theme allows you to create single page html sites suitable as a landing
page for [Syzygy](https://syzygy.ca) or [Callysto](https://callysto.ca)
instances. The landing page is constructed from widgets (inspired by
[wowchemy/academic](https://wowchemy.com/). The basic idea is to create widgets
under `content/home` which use one of the following widget templates

* [about](./layouts/partials/widgets/about.html): Two column favicon list of
  items
* [logos](./layouts/partials/widgets/logos.html): Two or three (or four) column
  list of logos
* [blank](./layouts/partials/widgets/blank.html): Single column content

Almost everything can be configured by either site wide `config.toml` or the
header of the content files.

## Usage
To start from scratch, create a new hugo site
```bash
$ hugo new site mysyzygy-site
```

Initiate the hugo module, this doesn't absolutely _have_ to correspond to an
existing remote repository, but it probably _should_.
```bash
$ cd mysyzygy-site
$ hugo mod init github.com/<your_user>/<your_project>
```

Add a config.toml which refers to the theme
```bash
$ vi config.toml
...
theme = ["github.com/pimsmath/gohugo-theme-syzygy-callysto"]
...
```

You should now be able to `hugo serve` the site. See the `exampleSite` directory
for common config options and content layouts, (don't copy the `theme` line from
there, it is configured for local development of the theme).
