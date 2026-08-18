# LJT-Homepage

Personal academic homepage of **Junteng Liu**, built with the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll
template and hosted with GitHub Pages.

## Content

| File / directory | Purpose |
| --- | --- |
| `_config.yml` | Site-wide settings and the sidebar author profile |
| `_pages/about.md` | Landing page: biography, education, research experience, skills, publications, contact |
| `_pages/cv.md` | Curriculum vitae |
| `_pages/publications.html` | Publications index (renders the `publications` collection) |
| `_publications/` | One Markdown file per publication |
| `_data/navigation.yml` | Header navigation links |

## Site URL

The site is configured with

```yaml
url:     https://lookoutlancer.github.io
baseurl: /LJT-Homepage
```

so it is served from `https://lookoutlancer.github.io/LJT-Homepage/`. If the
repository is renamed, update `baseurl` and `repository` in `_config.yml` to match.

## Running locally

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

See the [Academic Pages documentation](https://academicpages.github.io/) for more
details on customising the template.
