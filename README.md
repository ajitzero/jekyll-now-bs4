![Jekyll Now + Bootstrap 4 Logo](logo.png)

> [Jekyll Now](https://github.com/barryclark/jekyll-now) is a forkable starter template for creating a Jekyll blog by [Barry Clark](https://github.com/barryclark).
>
> This project is a clone of `barryclark/jekyll-now` from [this commit](https://github.com/barryclark/jekyll-now/tree/12cb8a2e97c3b63c4bc92d2a1ab050b35bf946b7).

# Jekyll Now with Bootstrap 4

In addition to the original features, this version includes some more features which I needed in multiple projects. Bootstrap is just handy.

## Features

- Uses [Bootstrap]([https://getbootstrap.com](https://getbootstrap.com/)) `4.3.1` layout.

- Supports **categories** as a [collection](https://jekyllrb.com/docs/collections/):
  - Each category gets a `/category/:name` page with meta-data.
  - `/category` lists all categories, along with all articles under them so far.
  
- Supports **authors** as a collection:
  - Each author gets a `/authors/:name` page with social links and bio.
  - `/authors` lists all authors. For now.
  
- Includes `/_data`, currently used for navigation links only.
  
  > This one isn't a "necessary" addition but allows for much freedom in the long run.
  > Or so I think 🙌
  
- Supports Profile Pictures, which falls back to a placeholder avatar with custom initials set in the author's markdown file.

- Plugins used:
  - `jekyll-paginate`: Pagination as `/articles/:num/`
  - `jekyll-mentions`: Support for mentions, defaulting to Twitter.
  - `jekyll-redirect-from`: Support for redirecting pages. Must-have, really.
  - `jekyll-gist`: Supports for gists.
  
- Basic styling options with Sass variables:

  - `primary-light` & `primary-dark`.
  - `accent`: This is the only one I've used everywhere.

------

### Notes

- This is by default meant for *user* or *organisation* websites, like `<username/org-name>.github.io`, just like Jekyll Now was made.

- For *project* websites, update `baseurl` in `_config.yml` as the repository name.

  **e.g.** If the name of the repository is assumed to be `repo` then the `baseurl` should be set as `/repo`, while the website can be viewed on `<username/org-name>.github.io/repo/`.

- **Removed** Disqus related code.

  > This part can be easily restored from [Jekyll Now](https://github.com/barryclark/jekyll-now). I don't ever use it though.

- `jekyll-avatar` was added, then **removed** later due to [this issue](https://github.com/benbalter/jekyll-avatar/issues/37).

- `/articles/index.html` is needed instead of a simpler `/articles.md` since `jekyll-paginate` requires an `index.html` file. No support for `*.md` 😔

## Meta

[![GitHub followers](https://img.shields.io/github/followers/AjitZero.svg?style=social&label=Follow&maxAge=2592000)](https://github.com/AjitZero?tab=followers)

Ajit Panigrahi – [@AjitZero](https://github.com/AjitZero) – Ping me on [Twitter](https://twitter.com/AjitZero) for any urgent queries, raise an issue for anything else.

Distributed under the [MIT License](https://opensource.org/licenses/MIT). See [`LICENSE`](https://github.com/AjitZero/jekyll-now-bs4/blob/master/LICENSE) for more information.
