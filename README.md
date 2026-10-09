# KP Muhurat Daily Schedule — New Project

This is a **separate project**. It does not overwrite or replace the existing KP Muhurat Web 2.0 files.

## Daily schedule view
The Results tab includes a separate table with:
- No.
- Combination
- Start Time
- Stop Time
- Total Minutes

It includes CSV export for Excel. The schedule view uses the included live KP calculation/transition functions; it does not insert a global +1-second adjustment or use hardcoded date-specific timestamps to generate the schedule.

## Important validation note
The UI and project separation are implemented, but exact equivalence with the Prophet Pilot screenshot has not yet been certified. Compare the same date, location, and time range against the reference app before relying on the output for timing decisions.

## Run
Open `index.html` in a modern browser. If browser restrictions prevent local calculation assets from loading, serve this folder using a static local web server or deploy the folder as its own separate site.

## Preservation
Keep the original `index.html` and `README.md` for KP Muhurat Web 2.0 in their original location. This folder is the new project.

## Mobile layout update
The Daily Combination Schedule table now fits phone screens by reducing padding and font size and wrapping combination names, while keeping all five columns visible without horizontal scrolling. This is a layout-only change; it does not change KP calculation or transition timing logic.
