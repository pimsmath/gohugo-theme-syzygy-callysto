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
