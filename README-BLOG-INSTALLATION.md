# ABUHANI.TECH Insights — GitHub Pages add-on

This ZIP contains **only the blog add-on**, not a replacement for the existing website.

## Included
- `blog/index.html`: blog homepage with search and category filters
- `blog/<article-slug>/index.html`: six starter articles
- `blog/assets/blog.css` and `blog/assets/blog.js`: blog-only styling and filtering
- `SITEMAP-ADDITIONS.xml`: URLs to merge into the existing sitemap (not a replacement sitemap)

## Install into the existing repository
1. Download and extract this ZIP on your computer.
2. Open the extracted `ABUHANI.TECH-BLOG-ADDON` folder.
3. In GitHub, open `AHthree/AbuHani.Tech` on the `main` branch.
4. Upload the **contents** of the extracted folder into the repository root. Do not upload the ZIP itself, and do not create an extra `ABUHANI.TECH-BLOG-ADDON/` folder.
5. When prompted, commit the changes. The upload should add a `blog/` folder and the `SITEMAP-ADDITIONS.xml` helper file. It should not overwrite `index.html`, `assets/style.css`, `assets/script.js`, or the current `sitemap.xml`.
6. After GitHub Pages deploys, check `https://ahthree.github.io/AbuHani.Tech/blog/`.

## Sitemap: do this after the blog works
Open the existing root `sitemap.xml`. Copy the six `<url>...</url>` entries from `SITEMAP-ADDITIONS.xml` and paste them **inside the existing `<urlset>...</urlset>`**, before its closing `</urlset>`. Do not copy the helper file's outer `<urlset>` tags, and do not replace the existing sitemap. Commit the sitemap change. Then inspect `https://ahthree.github.io/AbuHani.Tech/sitemap.xml`.

## Add a Blog link to the main navigation
This add-on does not overwrite the homepage. To link to the blog, edit the existing root `index.html` and add a navigation link like `<a href="blog/">Insights</a>` beside the existing navigation links. The exact location depends on the existing nav markup. Do not replace the whole homepage with the blog index.

## Important notes
- The six starter articles are new general educational drafts. They are **not imported from Base44** because no source/export was available. Review and personalize them before publishing as final company advice.
- Update the publication date when an article is substantively reviewed and published.
- The canonical URLs are set for the current GitHub Pages URL: `https://ahthree.github.io/AbuHani.Tech/`.
- The site is static and does not need a paid Base44 domain integration. GitHub Pages serves static HTML/CSS/JS from the repository.
- This is an additive package: only upload its contents into the existing repository root.
