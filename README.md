# maymo

Brown dwarf polar vortex modeling — multi-epoch atmospheric simulations for substellar objects.
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

---

University of Arizona · MIT License
