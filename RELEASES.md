# Release history

Downloads: [GitHub Releases](https://github.com/squintz-sol/HornPub/releases).

## v0.3.9 (pre-release), first public release

**New**
- **Rolling EXP/hour:** the dashboard shows your EXP rate over the last 10 minutes (choose 5 / 10 / 15 / 30).
  After Stop, the final rolling rate is kept and labelled "Final · 10 min", and it's still there after a
  restart. The whole-session average is in the tooltip and in History.
- **Level-up ETA:** uses its own 15-minute rolling rate. It shows *measuring* until 5 minutes of EXP have been
  measured, instead of guessing.
- **Custom EXP target:** Next Level or any % you type, with time left and the local arrival time.
- **Top 3 Farming Maps:** rank by EXP/hr, Mesos/hr or Net Mesos/hr, using each map's best recording or its
  average.
- **Map Performance filters:** by map and period (All Time, Today, Last 7 / 30 Days, custom range); recordings
  that run past midnight are split at midnight.
- **Minimap thumbnails:** each map's picture is taken from its expanded minimap. A reminder appears after
  about 10 minutes on a map without a picture.
- **ⓘ Help:** a built-in Getting Started guide.

**Improved**
- **Potions:** switch potions mid-recording; a large jump in a potion count is flagged as a possible restock,
  not counted as potions picked up.
- **Net Mesos:** farming earnings and your actual wallet change are kept apart.
- **History:** a consistent light theme, even with Windows dark mode.

**Fixed**
- Levels containing a 7 (37, 47, 57, …) could be read with a digit missing. Saved recordings now show the level
  their EXP indicates.
- EXP gained across a short gap in screen readings no longer causes a spike in the rolling rate.

## Earlier versions

Versions 0.1 to 0.3.8 were private test builds and were not published.
