<a href="https://photon-platform.net/">
    <img src="https://photon-platform.net/user/images/photon-logo-banner.png" alt="photon" title="photon" align="right" height="120" />
</a>


# photon ✴ Home

## 0.1.0

---


> Home page for photon

- [configuration](#configuration)
- [templates](#templates)
- [scaffolds](#scaffolds)
- [scss](#scss)
- [assets](#assets)
- [languages](#languages)

# configuration
blueprints.yaml

fields:
- enabled
- built_in_css
- built_in_js

Before configuring this plugin, you should copy the `user/plugins/photon-home/photon-home.yaml` to `user/config/plugins/photon-home.yaml` and only edit that copy.

Here is the default configuration and an explanation of available options:

```
enabled: true
built_in_css: true
built_in_js: true

description: Custom Text added by the **photon-home** plugin (disable plugin to remove)
```

Note that if you use the admin plugin, a file with your configuration, and named photon-home.yaml will be saved in the `user/config/plugins/` folder once the configuration is saved in the admin.


# blueprints

```sh
blueprints
└── home.yaml
```

### Home
home.yaml
extends: article
fields:
- home
  - header.content.items

# templates

```sh
templates
├── _articles
│   ├── _block
│   │   ├── article_figure_showcase.html.twig
│   │   ├── article_footer_showcase.html.twig
│   │   ├── article_header_showcase.html.twig
│   │   └── article_main_showcase.html.twig
│   ├── article-showcase.html.twig
│   └── home.html.twig
├── _sections
│   ├── featured.html.twig
│   └── showcase.html.twig
├── home.html.twig
├── home-orig.html.twig
└── README.md
```
The primary difference of the Home page from the parent Article page is the Showcase and Featured panels.

# scss

```sh
scss
├── articles
│   ├── _article-showcase.scss
│   └── _home.scss
├── templates
│   └── home
│       ├── _featured.scss
│       ├── _index.scss
│       └── _showcase.scss
└── home.scss
```

# assets

```sh
assets
├── home.css
├── home.css.map
├── home.js
└── showcase.js
```

# languages

```sh
languages
└── en.yaml
```


## Installation

- all photon plugins are installed as git submodules. More on that later.



## Configuration


## Usage

Select template type when creating a new page

## Credits


## To Do

- [ ] Future plans, if any


copyright &copy; 2020
