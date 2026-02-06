# Multiplier and Acceleration Principle — Chow (1968)

**Gregory C. Chow, "Multiplier, Accelerator, and Liquidity Preference in the Determination of National Income in the United States"**

> *The Review of Economics and Statistics*, Vol. 49, No. 1 (Feb., 1967), pp. 1–15.

## About

This repository contains a MyST Markdown reproduction of Gregory C. Chow's 1968 paper on the acceleration principle published in *The Quarterly Journal of Economics*. The paper has been converted from PDF to a web-readable format using [MyST Markdown](https://mystmd.org/).

## Project Structure

```
├── original/               # Original PDF (preserved)
├── paper/                  # MyST paper source
│   ├── paper.md            # Main paper in MyST Markdown
│   ├── references.bib      # Bibliography
│   └── figures/            # Extracted figures
├── docs/                   # Documentation
│   └── index.md            # Landing page
├── myst.yml                # MyST configuration
└── README.md
```

## Building

```bash
# Install MyST
npm install -g mystmd

# Build HTML
myst build --html

# Start dev server
myst start
```

## License

The original paper is reproduced for academic and educational purposes.
