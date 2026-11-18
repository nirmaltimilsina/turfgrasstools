# Turfgrass Tools website

Public website for Turfgrass Tools, independently developed by Nirmal Timilsina.

Live site: https://nirmaltimilsina.github.io/turfgrasstools/

This repository should contain **only these public website files**:

- `index.html`: homepage, tool descriptions and status labels.
- `config.js`: deployed Streamlit app links.
- `favicon.svg`: site icon.
- `README.md`: this file.

Each Python application lives in its own **private** GitHub repository. Do not upload `app.py`, `model.py`, research datasets, private API keys, or `secrets.toml` here.

## Turn on a tool link

The homepage links to four currently deployed calculators. To change an app's address, edit `config.js`. Example:

```js
window.TURFGRASS_TOOL_URLS = {
  pgr: "https://turf-pgr-gdd.streamlit.app/",
  gp: "https://turf-growth-potential.streamlit.app/",
  nitrogen: "https://turf-nitrogen-planner.streamlit.app/",
  irrigation: "https://turf-irrigation.streamlit.app/"
};
```

The homepage automatically hides any link with an empty URL. Growth Monitoring, Stress Assessment, and Disease Risk remain listed as under development, without public launch links.

## GitHub Pages settings

Repository: `turfgrasstools` (Public). Under **Settings → Pages**, choose **Deploy from a branch**, `main`, `/(root)`. The site updates after a new commit and deployment. If changes do not appear immediately, wait for Pages to finish publishing and refresh the browser.

No domain purchase or paid web hosting is needed to use the GitHub Pages address.
