# PDF Editor — changelog

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
