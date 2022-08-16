# Ataraxia

A personal theme for [Zola](https://www.getzola.org/) focused on readability that aims to be simple, beautiful, and modern. It is designed to support multiple languages and be highly customizable.

The theme takes visual inspiration from the [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) and [Neumorphism](https://github.com/longpdo/neumorphism) themes.

## Installation

Open a command terminal at your site path and run:

```console
cd themes
```

```console
git clone https://github.com/gersonbdev/ataraxia-zola.git
```

## Configuration

Copy the `config_sample.toml` file to your site's main path, then rename it to `config.toml` and edit it with your site data.

> You can see the [Gerson's website](https://github.com/gersonbdev/gersonbdev.github.io) repository for theme setup guide.

For the site to work properly you need to create a `_index.md` file within the `content` path with the following structure:

```toml
+++
title = "Home"
description = "Home site description."
sort_by = "date"
template = "index.html"
page_template = "page.html"
+++
```

You can add more markdown content inside this file if you need to.

If you want to enable the site's blog, create a _index.md file inside the `content/blog` path then copy the following structure inside the file:

```toml
+++
title = "Blog"
description = "Blog site description."
sort_by = "date"
paginate_by = 5
template = "blog.html"
page_template = "blog_page.html"
+++
```

You can display the result of your website by running:

```console
zola serve
```


## Hacking

By default, the theme comes with all the scss styles already compiled, in such a way that the installation of Bootstrap is not necessary, in order to avoid dependencies such as Node.js in the production file.

If you want to edit the theme's styles, you'll need to have a [Node.js](https://nodejs.org/) interpreter and a [Sass compiler](https://sass-lang.com/install) installed. After that, go to the main path of the theme and execute:

```console
npm install
```

```console
sass --watch scss/custom.scss:static/assets/css/custom.css
```

> Keep in mind that the main branch of this repository only has the stable versions of the theme, if you want to see the development status and the unstable versions, change to the corresponding branch.

## Credits

This theme is mainly built on [Zola](https://www.getzola.org/) and [Bootstrap](https://getbootstrap.com/), plus it makes use of [Google fonts](https://fonts.google.com/).


## Sponsoring
[![Liberapay](https://img.shields.io/badge/Finance%20the%20project-F6C915?style=flat&logo=liberapay&logoColor=ffffff "Finance the project")](https://liberapay.com/gersonbenavides/donate)


## License

This work is published under the [MPL-2.0](https://www.mozilla.org/en-US/MPL/2.0/) license