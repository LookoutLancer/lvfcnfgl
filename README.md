# LJT-Homepage

Personal academic homepage of **Junteng Liu**, built with the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) Jekyll
template and hosted on GitHub Pages.

## Content

| File / directory | Purpose |
| --- | --- |
| `_config.yml` | Site-wide settings and the sidebar author profile |
| `_pages/about.md` | Landing page: biography, research interests, education, research experience, award, skills, publications, contact |
| `_pages/cv.md` | Curriculum vitae |
| `_pages/publications.html` | Publications index (renders the `publications` collection) |
| `_publications/` | One Markdown file per publication |
| `_data/navigation.yml` | Header navigation links |

All personal data on this site comes from a single source and nothing has been
invented: no placeholder authors, papers, dates or links from the upstream
template remain.

## Site URL

```yaml
url:      https://lookoutlancer.github.io
baseurl:  /LJT-Homepage
repository: LookoutLancer/LJT-Homepage
```

`baseurl` **must match the repository name** — it is the subpath GitHub Pages
serves a project site from. The values above are correct for the intended
repository name, `LJT-Homepage`.

If the repository name changes, update `baseurl` and `repository` in
`_config.yml` to match, otherwise every link and asset on the site will 404.

## Not yet finished: verify your email address

The GitHub account that owns this repository has **no verified email address**,
and GitHub blocks repository creation, forking, renaming and Pages builds until
one is verified. Every such action fails with:

```
403 At least one email address must be verified to do that.
```

Because of this the repository could not be created under the name
`LJT-Homepage`; it currently lives in the placeholder repository it was built
into. To finish the setup:

1. Verify an email address at **https://github.com/settings/emails**.
2. Rename the repository to **`LJT-Homepage`**
   (*Settings -> General -> Repository name*).
3. Nothing else is needed — GitHub Pages is already enabled on `main` and will
   build automatically. The site will then be live at
   `https://lookoutlancer.github.io/LJT-Homepage/`.

> Until step 1 is done, GitHub Pages will report the build as `building`
> indefinitely and the site URL will return 404. This is expected, not a
> misconfiguration of the site itself.

## Running locally

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

For local previews against the current repository name, override the base path:

```bash
bundle exec jekyll serve --baseurl /LJT-Homepage
```

See the [Academic Pages documentation](https://academicpages.github.io/) for more
details on customising the template.
