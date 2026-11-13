# Ikechukwu Festus Okeke — Portfolio Website

A single-page, fully static portfolio website built with plain HTML and CSS — no
build step, no dependencies, no JavaScript frameworks.

**Live URL (once GitHub Pages is enabled):**
<https://okekefestus0-max.github.io/my_portfolio-/>

## What's in the repo

| File                             | Purpose                                                     |
| -------------------------------- | ----------------------------------------------------------- |
| `index.html`                     | The website (entry point served by GitHub Pages)            |
| `favicon.svg`                    | Browser tab icon — "IFO" monogram                           |
| `.nojekyll`                      | Tells GitHub Pages to serve the files as-is, without Jekyll |
| `Ikechukwu_Okeke_Portfolio.html` | Original uploaded copy of the page (kept for reference)     |

> `index.html` is the source of truth. If you edit your content, edit
> `index.html`.

## Sections

- **Hero** — intro and call-to-action links (email, LinkedIn)
- **About** — background, education and current focus
- **Skills** — cybersecurity training, computer engineering/ICT, digital
  marketing interests, digital and web tools
- **Experience** — NYSC Financial Inclusion CDS presidency, class representative
- **Education** — HND, Tech4Youth training, certificates
- **Contact** — email, LinkedIn, phone and location

## Run it locally

Any static file server works. From the repository root:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

Alternatively, just double-click `index.html` to open it in a browser.

## Publish it on GitHub Pages

1. On GitHub, open this repository and go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to _Deploy from a branch_.
3. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
4. Wait a minute or two, then visit
   <https://okekefestus0-max.github.io/my_portfolio-/>.

## Editing the content

Everything lives in one file. Text is in the `<body>`; colours, spacing and the
responsive layout are in the `<style>` block in the `<head>`. The colour palette
is defined once as CSS variables:

```css
:root {
  --bg: #0b1220; /* page background   */
  --panel: #131e31; /* card background   */
  --ink: #eaf2ff; /* main text         */
  --muted: #aab9cf; /* secondary text    */
  --accent: #67e8c5; /* links and buttons */
}
```

Change a value there and the whole site updates.

## Custom domain (optional)

To use your own domain, add a `CNAME` file containing the domain (for example
`ikechukwuokeke.dev`), then point a `CNAME` DNS record at
`okekefestus0-max.github.io`.
