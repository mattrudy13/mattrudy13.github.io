# mattrudy13.github.io

Portfolio site for Matthew Rudisill, aimed at recruiters: skills, day job, and projects.
Live at https://mattrudy13.github.io/

Plain HTML and one stylesheet, no build step. GitHub Pages serves `main`.

- `index.html`: masthead (intro, skills, contact links), at work, featured project, more projects, contact
- `style.css`: shared styles (light, plus a dark version that follows the system setting; the ☾/☀ button
  at the end of the top bar overrides it and is saved in the browser as `portfolio:theme`)
- `Matthew-Rudisill-Resume.pdf`: the public resume, linked in the top bar and Contact. It's a web copy with
  no phone or email (LinkedIn instead). The original Word export's PDF title was fixed in place to
  "Matthew Rudisill Resume" so the browser tab reads cleanly. Other resume PDFs in this folder are
  ignored by `.gitignore` so the copy with a phone number never gets committed.
- `img/`: project screenshots of the live sites in light mode, taken at 840×630 (2× scale) and saved
  as 1000×750 JPEGs. The apartments shot was taken with Playwright (from the apartments venv) so the
  temporary stale-pull `.banner` could be hidden; the others with headless Chrome
  (`--blink-settings=preferredColorScheme=1`, or they come out dark when macOS is in dark mode).
  `uva-records.jpg` (dashboard) and `kotc-tracker.jpg` (Tonight, Oct 21, 2026) were added for v0.3 the
  same way. `kotc-tracker.jpg` was re-shot on Oct 27, 2026 after its v0.6 redesign, with Playwright: scrolled
  to the "Main event" picks (the poster masthead alone fills the frame) with `#hero` and `#live-card` hidden
  so the frame ends on a section heading. `h2h.jpg` was re-shot on Oct 27, 2026 after its v0.2 redesign, and
  `uva-records.jpg` on Oct 28, 2026 after its v0.2 redesign (headless Chrome, dashboard, the usual 840×630 at 2×). `out-and-about.jpg` was added on Nov 4, 2026 (headless Chrome, the usual 840×630 at 2×). nba-first-minute and
  cbb-scores are left off on purpose, so the sports and betting projects don't dominate the page;
  beat-the-model gets a sentence and a link in the cfb-picks case study instead of a card. The hub is personal,
  not for recruiters.

The work section stays generic: no employer name and no internal app names. The featured chart's
numbers come from `cfb-picks/data/backtest.json` (v1) and `backtest-v3.json` (v2 and v3). The reason
under each bar: v1 was under 52.4%; v2 was profitable in only 2 of 4 seasons (`backtest-v2.json` →
`profitableSeasons`), against the bar of 3; v3 made 3 (`backtest-v3.json`). The page carries no live
record, since it goes stale; "See the live record" links to the cfb-picks site.
