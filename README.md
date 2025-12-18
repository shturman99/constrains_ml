# Constraint-Preserving DNS + ML Draft

This repository contains an Overleaf-ready LaTeX project for a research draft on machine learning methods that accelerate constraint enforcement in incompressible Navier--Stokes and MHD direct numerical simulations.

## Structure
- `main.tex`: entry point including packages and bibliography.
- `macros.tex`: reusable macros.
- `sections/`: separate section files (abstract, introduction, problem setup, taxonomy, related work, plan, experiments, risks, conclusion).
- `references.bib`: curated bibliography.
- `fig/`: placeholder for figures.

## How to compile
Use pdfLaTeX (or Overleaf's default) to compile `main.tex`. Ensure `natbib` is enabled for citations.

## Editing guide
- Update text within `sections/` files; keep `main.tex` minimal.
- Replace the placeholder figure reference in `sections/03_methods_taxonomy.tex` with an actual schematic saved under `fig/`.
- Adjust macros or add new ones in `macros.tex`.

## Next steps checklist
- Select target PDE cases (e.g., Taylor--Green vortex, Orszag--Tang vortex, channel flow).
- Choose datasets or generate DNS snapshots; define train/validation splits.
- Implement baseline solvers (pseudo-spectral and finite-volume) with projection/CT.
- Pick ML strategy (neural operator + projection, divergence-free network, learned multigrid) and configure losses.
- Define logging, seeds, and hardware assumptions.

## Bibliography curation
References include seminal projection/CT/divergence-cleaning papers and recent ML approaches (PINNs, neural operators, learned multigrid). Each citation contains venue and DOI/URL when available for quick lookup.
