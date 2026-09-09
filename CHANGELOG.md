# PDF Editor — changelog

## 0.1.6 — 2026-09-09

**Installer:** re-running the installer over an existing copy now offers an
**Update** option (selected automatically when it detects an older version
already installed) alongside Full install and Unzip.

Background color tweak, mostly to give this release something visible to
confirm the in-app updater actually applied it.

## 0.1.5 — 2026-09-09

Fixes the in-app updater itself: the app could still be closing when the
installer tried to replace its files, and the update would silently do
nothing — no error, just no update. The app now closes immediately once the
installer starts, so this can't happen.

## 0.1.4 — 2026-09-09

The update check now runs every time you open the app, not just once a day —
so if a new version is out, you'll see the prompt right when you launch
instead of having to open About and click **Check for updates** yourself.

## 0.1.3 — 2026-09-09

**Smoother updates.** The "update available" prompt now comes forward on its
own instead of waiting behind the window, and a small progress window shows
each step — downloading (with a percentage), verifying, then restarting — so
a download is never a blank wait.

**Send feedback.** A new option in the About dialog (bug / idea / comment) —
report something without leaving the app. Your version is attached
automatically; nothing else about your files or work is sent.

Under the hood: the startup update check now carries a random ID so active
installs can be counted (no personal data). See the privacy note on
unsubbedware.com/about.

## 0.1.1 — 2026-09-07

Adds an About dialog — reach it from the version chip in the top-right corner
or the illustration on the start screen. It shows the version, links to
unsubbedware.com, and has a **Check for updates** button.

Also a redrawn start screen: an illustration and the app name in place of the
plain document icon.

## 0.1.0 — 2026-09-07

First public beta.

A local, offline desktop PDF editor for Windows — no cloud upload, no account.

**Pages**
- Open and view PDFs (continuous scroll or one-page-at-a-time), true physical-size zoom, Normalize-to-A4 view.
- Organize view: reorder, delete, insert blank pages, and merge in other PDFs by drag-and-drop.
- Per-page rotate, flip, resize, and content repositioning.

**Fill & Sign**
- Place freeform text anywhere on a page.
- Add a date with a chosen format.
- Add a signature — draw it, load an image, or generate one from a typed name — and reuse it from a saved library.

**Markups**
- Comment pins, pen, rectangles, ellipses, arrows, and text highlight / underline / strikethrough.
- Threaded comments with a review panel and per-markup status (needs changes / has questions / resolved).
- Markups round-trip with Adobe Acrobat — open a file marked up in Acrobat, reply to its comments, and save back.

**Saving**
- Save writes text, dates, signatures, and markups back as real, editable PDF annotations.
- Export produces a flattened PDF, or a PNG / JPEG, with toggles for baking annotations and including markups.

Known limitations in this beta: real AcroForm form-field filling isn't implemented yet (use freeform text to fill any PDF); the installer is unsigned, so Windows SmartScreen will show an "unknown publisher" warning.
