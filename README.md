# rejikjoseph.com

Personal academic website of Reji K. Joseph, built with the
[Academic Pages](https://github.com/academicpages/academicpages.github.io) template
and hosted free on GitHub Pages.

## Where the content lives

| Menu tab        | File to edit                  |
|-----------------|-------------------------------|
| About (home)    | `_pages/about.md`             |
| Publications    | `_pages/publications.md`      |
| Talks           | `_pages/talks.md`             |
| Teaching        | `_pages/teaching.md`          |
| Opinion Pieces  | `_pages/opinion-pieces.md`    |

- Menu order: `_data/navigation.yml`
- Name, sidebar text, links (Google Scholar, ORCID, email…): `_config.yml` (the `author:` section)
- Profile photo: replace `images/profile.png` (square image, about 400×400 px)
- Book covers: `images/books/`

## Adding a new entry

Open the file on GitHub, click the pencil icon, add a paragraph under the right
year (newest first), and click **Commit changes**. The site updates in 1–2 minutes.

Formatting:

- `**Bold title**` → bold
- `*Journal or event name*` → italic
- `[**Title**](https://link)` → linked title

Example (Talks):

    **Title of the Talk**, *Name of the Conference*, Organiser, City, 12 March 2027.

For a new year, add a heading `## 2027 {#y2027}` (use `###` on the Publications
page) and add `2027` to the year links line at the top of that page.

## Publishing (one-time setup)

1. Create a GitHub account and a **public** repository named
   `YOUR-USERNAME.github.io`.
2. Upload all files from this folder (Add file → Upload files; drag the contents in).
3. In `_config.yml`, replace `YOUR-GITHUB-USERNAME` in the `repository:` line.
4. Settings → Pages → Build and deployment: Source **Deploy from a branch**,
   branch **main**, folder **/ (root)**.
5. Settings → Pages → Custom domain: `rejikjoseph.com` → Save. Tick
   **Enforce HTTPS** once it becomes available.
6. At GoDaddy (My Products → rejikjoseph.com → DNS), remove any existing
   parked/forwarding `A` record for `@` and add:
   - `A` records for `@` → `185.199.108.153`, `185.199.109.153`,
     `185.199.110.153`, `185.199.111.153`
   - `CNAME` record for `www` → `YOUR-USERNAME.github.io`

DNS changes can take a few hours to take effect.
