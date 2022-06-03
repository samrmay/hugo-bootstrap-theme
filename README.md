# Hugo Bootstrap Theme

[![Build and Deploy to gh-pages branch](https://github.com/filipecarneiro/hugo-bootstrap-theme/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/filipecarneiro/hugo-bootstrap-theme/actions/workflows/gh-pages.yml) [![Publish to GitHub Pages](https://github.com/filipecarneiro/hugo-bootstrap-theme/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/filipecarneiro/hugo-bootstrap-theme/actions/workflows/pages/pages-build-deployment)

Theme for a blazing fast static website and/or blog using bootstrap 5.

![Screenshot](images/tn.png)

## Demo

- [https://filipecarneiro.github.io/hugo-bootstrap-theme/](https://filipecarneiro.github.io/hugo-bootstrap-theme/)

## Features

- 🛡️ Security aware
  
  Get A+ scores on Mozilla Observatory out of the box. Easily change the default Security Headers to suit your needs.

- ⚡Fast by default
  
  Get 100 scores on Google Lighthouse by default. Hugo Bootstrap Theme removes unused css, prefetches links, and lazy loads images.
  
- 📈 SEO-ready
  
  Use sensible defaults for structured data, open graph, and Twitter cards. Or easily change the Search Engine Optimization settings to your liking.

## Framework

### Hugo

Hugo is the **world’s fastest static website engine**. It’s written in Go (aka Golang).

- [Hugo Documentation](https://gohugo.io/documentation/)

- [Go template documentation](https://golang.org/pkg/text/template/#hdr-Functions)

### Bootstrap

Get started with Bootstrap

- [Bootstrap 5.2](https://getbootstrap.com/docs/5.2/getting-started/introduction/)

- [Install Bootstrap in your Node.js powered apps with the npm package](https://getbootstrap.com/docs/5.2/getting-started/download/#npm)

### Requirements

The tools used are cross-platform and should work on Windows, MacOS and Linux. You will need the following tools to be downloaded and installed:

- [Hugo static site builder](https://github.com/goHugoio/Hugo/releases) - IMPORTANT: make sure you pick the extended version, Hugo_extended_0.xx.x_…

- [Node & NPM](https://nodejs.org/) - We use this to maintain project dependencies

- [Git](https://git-scm.com/downloads) - This is optional, but highly recommended for version control and remote backups.

## Usage

### Test the theme locally on your computer

Clone this repo:

```
git clone https://github.com/filipecarneiro/hugo-bootstrap-theme.git
```

Test if the site is working:

```
hugo server -D --disableFastRender --source exampleSite
```

This launches Hugo development server and you can see the example site by opening http://localhost:1313/hugo-bootstrap-theme/.

### Install on an existing Hugo site

#### Step 1: Install via NPM

```
npm install @filipecarneiro/hugo-bootstrap-theme
```

Hugo bootstrap theme package will also add bootstrap and feather-icons to node modules.

#### Step 2: Add to Config

Then add the theme `hugo-bootstrap-theme` to your sites [configuration file](https://gohugo.io/getting-started/configuration/#configuration-file) `config.toml`, `config.yaml` or `config.json`:

```toml
theme = "hugo-bootstrap-theme"
themesdir = "node_modules\\@filipecarneiro"
```

The new themes directory (themesdir) is needed to get the new theme from the `node_modules` folder.

#### Step 3: Test your site

```
hugo server -D --disableFastRender
```

#### Step 4: Check your parameters

Check your `copyright` variable, your menus (the theme supports `main`, `footer` and `social` menus), etc.

Have a look on exampleSite for inspiration :)
