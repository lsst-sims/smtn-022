[![Website](https://img.shields.io/badge/smtn--022-lsst.io-brightgreen.svg)](https://smtn-022.lsst.io)
[![CI](https://github.com/lsst-sims/smtn-022/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sims/smtn-022/actions/workflows/ci.yaml)

# Integrating LightCurveLynx with MAF

## SMTN-022

The Metrics Analysis Framework (MAF) supports evaluation of simulated (or real) Rubin pointing histories for a wide variety of science cases, primarily using basic information about the visit metadata itself. LightCurveLynx (LCL) supports the creation of flux time series data (lightcurves) from such pointing histories. 

Integrating LCL with MAF to go seamlessly from a transient or variable model available in LCL to the lightcurve data to a figure of merit for a given pointing history enables the evaluation of a wider range of transient and variable science to help guide survey strategy or science investigations. 

This technote describes the integration of these two software packages, LCL and MAF, along with design choices in this integration.

**Links:**

- Publication URL: https://smtn-022.lsst.io
- Alternative editions: https://smtn-022.lsst.io/v
- GitHub repository: https://github.com/lsst-sims/smtn-022
- Build system: https://github.com/lsst-sims/smtn-022/actions/


## Build this technical note

You can clone this repository and build the technote locally if your system has Python 3.11 or later:

```sh
git clone https://github.com/lsst-sims/smtn-022
cd smtn-022
make init
make html
```

Repeat the `make html` command to rebuild the technote after making changes.
If you need to delete any intermediate files for a clean build, run `make clean`.

The built technote is located at `_build/html/index.html`.

## Publishing changes to the web

This technote is published to https://smtn-022.lsst.io whenever you push changes to the `main` branch on GitHub.
When you push changes to a another branch, a preview of the technote is published to https://smtn-022.lsst.io/v.

## Editing this technical note

The main content of this technote is in `index.md` (a Markdown file parsed as [CommonMark/MyST](https://myst-parser.readthedocs.io/en/latest/index.html)).
Metadata and configuration is in the `technote.toml` file.
For guidance on creating content and information about specifying metadata and configuration, see the Documenteer documentation: https://documenteer.lsst.io/technotes.
