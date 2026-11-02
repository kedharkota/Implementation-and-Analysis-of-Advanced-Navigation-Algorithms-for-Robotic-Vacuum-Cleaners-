# Reproducibility and visual sources

## Scope

This guide describes what is available in the committed project and what is required to reproduce it. The documentation update inspected source and saved outputs; it did not rerun model training or hardware/simulation experiments.

## Required inputs

Reproduction requires the original Webots scene and controller implementations, plus scenario definitions and metric calculations. The separate `webots` repository on this account is an upstream simulator fork and does not by itself establish that this project's controller source is available.

## Entry point

Begin with `Final_Review.pdf` for the project's objectives, methods, and simulation results. Use `Report.docx` and `Research_paper.pdf` for the accompanying written material.

This checkout contains documents only. To rerun the simulation, restore the corresponding Webots world, robot configuration, controller source, assets, and version information; those files are not committed here.

## Evidence and interpretation

The map preview above is extracted from page 8 of the committed final review. Algorithm names reflect the project material, while executable implementations and raw comparison tables are absent from this checkout. The README therefore presents this as a study archive.

## Visual provenance

All screenshots and experiment figures are tied to repository material. Workflow SVGs are explanatory illustrations. The full image inventory is in [assets/sources.json](assets/sources.json).

| Visual | Source |
| --- | --- |
| [overview.svg](assets/overview.svg) | New explanatory project-workflow diagram based on the committed source and documentation; not a screenshot or measured result. |
| [simulation.png](assets/simulation.png) | Final_Review.pdf, page 8, embedded image X4.jpg |

## Validation

```bash
python tools/check_docs.py
```

The standard-library checker validates README/docs local link destinations and SVG/PNG/JPEG headers. It makes no external requests and installs no project runtime dependencies. External web links, model accuracy, image semantics, and full application execution need separate review.

## Reproduction record

For a new experiment or demo, record the source commit, environment versions, data provenance and split, configuration, command/notebook order, and resulting artifacts. Only label a measurement as reproduced after completing that run. Keep credentials and restricted datasets outside version control.
