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

After an app is deployed, has been tested, and is set to public in Streamlit Community Cloud, open `config.js` and enter its live HTTPS URL. Example:

```js
window.TURFGRASS_TOOL_URLS = {
  pgr: "https://turf-pgr-gdd.streamlit.app/",
  gp: "https://your-growth-potential-app.streamlit.app/",
  nitrogen: "",
  monitor: "",
  irrigation: ""
};
```

The homepage automatically changes that card from **In development** to **Available** and adds an **Open** link. Keep the URL empty until the app is live. The current PGR link is already configured.

## GitHub Pages settings

Repository: `turfgrasstools` (Public). Under **Settings → Pages**, choose **Deploy from a branch**, `main`, `/(root)`. The site updates after a new commit and deployment. If changes do not appear immediately, wait for Pages to finish publishing and refresh the browser.

No domain purchase or paid web hosting is needed to use the GitHub Pages address.
