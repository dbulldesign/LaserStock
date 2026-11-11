# LaserStock

Sheet nesting calculator for laser cutting circles. Enter a stock sheet and the
circles you need; it works out how many sheets to use and order, and lays the
circles out in even grids.

Current version: **1.13.0**

## Versions

- **1.13.0** — Shared stock through GitHub: everyone sees the same materials and counts; changing them needs a GitHub key. Every change is a commit on the `stock-data` branch, and simultaneous changes are merged.

- **1.12.0** — Spacing shown and editable in both mm and inches side by side; switching page units no longer rounds the spacing.

- **1.11.0** — Preset size buttons (MR16 = 1.9375", save your own); circle rows take the quantity first, then the diameter.

- **1.10.0** — Materials are a type plus a variant (Fade Not Poly - R02, Brightview - Wide…). Adding a variant picks up the type's sheet and cut size. Size list grouped by type with a Find material search; the Stock dialog has its own search. Job files remember the exact material.

- **1.9.0** — Materials & stock: save each material (sheet size, optional cut size, notes), track full sheets and spare cut pieces on hand with a reorder level, see In stock / After this job / To order for each job, mark jobs as cut, receive sheets, history with undo, export/import. Stock is kept in the browser.

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

## Shared stock

Materials, stock counts, preset sizes and the stock history live in `stock.json` on the
`stock-data` branch of this repository (kept apart from `main`, so stock changes never
rebuild the site). Anyone can view it. To change stock, open **Stock → Add GitHub key**
and paste a key with write access to this repository:

- **Repository owner:** a fine-grained token limited to this repository with
  *Contents: Read and write*.
- **Collaborators:** a classic token with the `public_repo` scope.

The key is kept only in that browser. Each change is saved as a commit under the key
owner's name, so the branch history is a full audit trail. The first time, someone with a
key clicks **Share this list** to start the shared file from their browser's list.

## Releasing

Bump `APP_VERSION` near the top of the script in `index.html` (and the version
above) whenever a change is merged to `main`. Open copies of the page notice the
new number and offer a reload.
