# Updating the portfolio

## Add a figure to a project
1. Export the plot or screenshot (PNG or JPEG, ideally under 200 KB, about 1200 px wide).
2. Put it in `assets/figures/` with a descriptive name, e.g. `mimosa-trajectory.png`.
3. In `README.md`, replace the placeholder line with
   `<img src="assets/figures/mimosa-trajectory.png" width="100%" alt="What the figure shows, in one sentence.">`
4. Add one sentence saying what the figure shows and one saying what it does not show (single run? seed? simulated or measured?).
5. Delete the placeholder image from `assets/placeholders/` if nothing else uses it.
6. Run `python3 tools/validate.py` before committing.

## Add a research entry
Replace the "Nothing is listed" paragraph in the Research section with one block per item:

```
**Title of the work**, authors. *Status label.* Venue or date. [Abstract](link) · [PDF](link) · [DOI](link)
```
Allowed status labels: published (peer-reviewed) · conference presentation · submitted manuscript · ongoing independent research · exploratory theoretical work. Never use "published" for anything that has not passed peer review.

## Keep "On my workbench" honest
Edit the three bullets whenever they stop being true. Only write what you are actually doing today. Remove "Where this page is thin" once the hardware work is documented.

## Regenerate the plots
`python3 tools/build_assets.py` rebuilds every image from `data/`. To make a new run of the QRNG simulation, run `run_sim_fixed.py` from `documentation/fixes/` inside a clone of the repository, copy `outputs/results.csv` to `data/qrng_run_fixed_seed7.csv` (or a new name and update the script), and rebuild.
Tools needed: `pip install numpy pandas matplotlib pillow playwright && playwright install chromium`.

## Hero and fonts
Typography: Fraunces (display), Source Serif 4 (italic text), Source Sans 3 and IBM Plex Mono (labels), all SIL Open Font License. Fonts are only used to render images, so visitors do not need them.
