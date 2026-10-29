<p align="center">
  <img src="assets/images/logo.svg" alt="IS-EUD logo" height="120">
</p>

<h1 align="center">IS-EUD Website</h1>

<p align="center">
  <a href="https://github.com/is-eud/is-eud.github.io/actions/workflows/jekyll.yml"><img src="https://github.com/is-eud/is-eud.github.io/actions/workflows/jekyll.yml/badge.svg" alt="Build & Deploy"></a>
  <a href="https://is-eud.github.io/"><img src="https://img.shields.io/website?url=https%3A%2F%2Fis-eud.github.io%2F" alt="Website status"></a>
</p>

Source of the IS-EUD website: <https://is-eud.github.io/>

Built with [Jekyll](https://jekyllrb.com/) and Bootstrap 6.

## Prerequisites

- Ruby 4.0 and Bundler
- Node.js 22 and npm

## Setup

```sh
bundle install
npm ci
```

`npm ci` also copies the Bootstrap JS bundle into `assets/js/vendor/` (gitignored) via a `postinstall` script.

## Run locally

```sh
bundle exec jekyll serve
```

The site is served at <http://localhost:4000> (unless a different port is specified using the `-P` option) and rebuilds on changes.

## Build and test

```sh
JEKYLL_ENV=production bundle exec jekyll build --baseurl ""
```

The output is written to `_site/`. There is no automated test suite: a change is considered good when this build succeeds and the result looks right when previewed (e.g. `python3 -m http.server -d _site`).

Every pull request to `main` runs this build in GitHub Actions and uploads `_site` as a preview artifact.

## Deployment

Pushing to `main` builds and deploys the site to GitHub Pages via GitHub Actions.

## Maintainers

<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%">
        <a href="https://github.com/espositoandrea">
          <img src="https://avatars.githubusercontent.com/espositoandrea?s=200" width="100px;" alt="Andrea Esposito"/>
          <br />
          <sub><b>Andrea Esposito</b></sub>
        </a>
      </td>
    </tr>
  </tbody>
</table>
