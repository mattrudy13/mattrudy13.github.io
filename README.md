# mattrudy13.github.io

Portfolio site for Matthew Rudisill, aimed at recruiters: skills, day job, and projects.
Live at https://mattrudy13.github.io/

Plain HTML and one stylesheet, no build step. GitHub Pages serves `main`.

- `index.html`: masthead (intro, skills, contact links), at work, featured project, more projects, contact
- `style.css`: shared styles (light only)
- `img/`: project screenshots of the live sites in light mode, taken at 840×630 (2× scale) and saved
  as 1000×750 JPEGs. The apartments shot was taken with Playwright (from the apartments venv) so the
  temporary stale-pull `.banner` could be hidden; the others with headless Chrome
  (`--blink-settings=preferredColorScheme=1`, or they come out dark when macOS is in dark mode)

The work section stays generic: no employer name and no internal app names. The featured chart's
numbers come from `cfb-picks/data/backtest.json` (v1) and `backtest-v3.json` (v2 and v3).
