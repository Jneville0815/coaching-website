# coaching-website

Jimmy's coaching and writing site, served at https://jimmyneville.com by GitHub Pages from `main` of the public repo `Jneville0815/coaching-website`. Plain HTML and one CSS file. There is no build step.

## Publishing

A push to `main` is a publish. After every change Jimmy asks for, commit to `main` and push in the same turn. The site updates within about a minute. Jimmy has given standing approval for this in this repo.

To preview before pushing, run `python3 -m http.server 8000` in this directory and open http://localhost:8000.

## Files

| Path | Holds |
| --- | --- |
| `index.html` | The coaching page |
| `blog/index.html` | The list of posts, newest first |
| `blog/_template.html` | The starting point for a new post |
| `blog/<slug>.html` | One file per post |
| `style.css` | All styles for every page |
| `favicon.svg` | The tab icon: a gold Bodoni Moda J, stored as a path |
| `CNAME` | The custom domain. Do not remove it |

## Copy

Jimmy writes all the copy. Use his words as given. Text in `[brackets]` is placeholder copy he has not written yet.

## Adding a post

1. Copy `blog/_template.html` to `blog/<slug>.html`, using a short kebab-case slug.
2. Fill in the title, description, date, and body.
3. Add an `<li>` for it at the top of the list in `blog/index.html`, and remove any placeholder `[bracketed]` posts still there:
   `<li><a href="/blog/<slug>.html"><time datetime="YYYY-MM-DD">Mon D, YYYY</time><h2>Title</h2><p>Standfirst.</p></a></li>`
