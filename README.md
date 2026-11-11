# LaserStock

Sheet nesting calculator for laser cutting circles. Enter a stock sheet and the
circles you need; it works out how many sheets to use and order, and lays the
circles out in even grids.

Current version: **1.8.0**

## Versions

- **1.8.0** — Staggered rows always run across the sheet width. Save and Open job files (.json) with every setting plus the calculated sheets and circle positions; Ctrl/Cmd+S and Ctrl/Cmd+O, or drop a file on the page.

- **1.7.0** — Layout switch: Best fit, Square or Staggered (straight rows, every other row shifted half a circle). Settings panel can be hidden and shown.

- **1.6.0** — Defaults: 10 mm from the sheet edge and 2 mm between circles; spacing shows its mm equivalent in inch mode.

- **1.5.0** — Type a unit with any size: `25mm`, `2.5cm`, `1 1/2"`, `2ft`. Circle rows switch to that unit; sheet and spacing values convert.

- **1.4.1** — Results update in place instead of blanking out, so the page no longer flashes or jumps when you change a setting.

- **1.4.0** — Each circle size can be entered in inches or millimetres.
- **1.3.0** — App icon, favicon and home-screen install.
- **1.2.0** — Circles are always laid out in even rectangular grids.
- **1.1.0** — Version number and update banner; Brightview is nested on 24 × 36 in
  cut sheets and the full 24 × 72 in sheets to order are shown.

## Releasing

Bump `APP_VERSION` near the top of the script in `index.html` (and the version
above) whenever a change is merged to `main`. Open copies of the page notice the
new number and offer a reload.
