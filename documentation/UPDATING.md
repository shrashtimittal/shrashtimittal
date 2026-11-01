# Updating the portfolio

## Add a figure to a project
1. Export the plot or screenshot (PNG or JPEG, ideally under 200 KB, about 1200 px wide).
2. Put it in `assets/figures/` with a descriptive name, e.g. `qrng-estimated-vs-true.png`.
3. In `README.md`, add an image tag using the relative path, for example:
   `<img src="assets/figures/qrng-estimated-vs-true.png" width="100%" alt="What the figure shows, in one sentence.">`
4. Add one sentence saying what the figure shows and one saying what it does not show (single run? seed? simulated or measured?).
5. Run the link and image-path checks before committing. The portfolio upload package does not include the asset-generation toolchain.

## Add a research entry
Replace the "Nothing is listed" paragraph in the Research section with one block per item:

```
**Title of the work**, authors. *Status label.* Venue or date. [Abstract](link) · [PDF](link) · [DOI](link)
```
Allowed status labels: published (peer-reviewed) · conference presentation · submitted manuscript · ongoing independent research · exploratory theoretical work. Never use "published" for anything that has not passed peer review.

## Keep "On my workbench" honest
Edit the three bullets whenever they stop being true. Only write what you are actually doing today.

## Regenerate the plots
`run_sim_fixed.py` documents the corrected bit-conversion path and runs the pseudo-random demonstration with seed 7. It expects the project modules (`sim` and `estimator`) from the QRNG repository, so it is not a standalone script. The README figures are static snapshots; regenerate them from the project repository when the underlying implementation changes.

## Hero and fonts
Typography: Fraunces (display), Source Serif 4 (italic text), Source Sans 3 and IBM Plex Mono (labels), all SIL Open Font License. Fonts are only used to render images, so visitors do not need them.
