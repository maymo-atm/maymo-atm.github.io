# maymo

Brown dwarf polar vortex modeling — multi-epoch atmospheric simulations for substellar objects.

**Website:** *(URL to be confirmed)*
**Docs:** `<site-url>/docs`
**GUI:** `<site-url>/gui`

---

## Repository structure

```
maymo/
├── index.html                  # Landing page 
├── gui/
│   └── index.html              # maymo-gui wrapper 
├── docs/                       # Sphinx build output → /docs
├── sphinx-src/                 # Sphinx source files (conf.py, rst/md, notebooks)
├── maymo/                      # Python package source
├── pyproject.toml
└── .github/
    └── workflows/
        └── deploy.yml          # GitHub Actions → GH Pages deploy
```

## Local development

Open `index.html` directly in a browser, or serve the repo root:

```bash
python -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

Push to `main`. The Actions workflow in `.github/workflows/deploy.yml` publishes the site automatically.

Before first deploy, enable GitHub Pages in your repo settings:  
**Settings → Pages → Source → GitHub Actions**

## Adding Sphinx docs

Once `sphinx-src/` is set up, uncomment the Python build block in `deploy.yml`. The workflow will run `make html` and copy the output into `docs/` on every push.

## maymo-gui

The JS app prototype lives in `gui/`. Point your compiled bundle at the `#app-mount` div in `gui/index.html`. The wrapper page shares the site navbar and can be developed independently of the Sphinx pipeline.

---

University of Arizona · MIT License
