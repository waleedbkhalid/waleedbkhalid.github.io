# Waleed Bin Khalid — personal website

A static academic site: plain HTML and CSS, with no build step or JavaScript.

## Structure

```
new_site/
├── index.html          Home: intro, affiliations, awards, research, teaching
├── projects.html       All projects, grouped by topic, with videos and images
├── css/
│   └── style.css       Shared styles for both pages
└── images/
    ├── profile.jpg     Portrait on the home page
    ├── logos/          Affiliation logos
    ├── research/       Thumbnails for the Research section
    └── projects/       Figures on the Projects page
```

## Editing

- Text lives directly in the two HTML files.
- To add an image, put it in the matching `images/` subfolder with a lowercase, hyphenated name (for example `images/projects/my-new-figure.png`) and reference it with that relative path.
- Fonts: Computer Modern loads from the jsDelivr CDN and falls back to Latin Modern, then Times New Roman.
- Videos are Google Drive and YouTube embeds, so they only play when the page is online.

## Preview locally

Open `index.html` in a browser, or run a small server from this folder:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Publishing

The folder works as-is on GitHub Pages or any static host. Upload the contents of `new_site/` so that `index.html` sits at the root of the site.
