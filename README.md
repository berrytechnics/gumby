# Classic Car Poster Builder

A single-file web app for designing vintage-style car posters and exporting them as PNGs.

## What It Does

- Live poster preview with editable content
- Multiple poster size presets + custom aspect ratio
- Theme presets with full color customization
- Reorderable spec sections and rows
- Per-row accent toggle for spec values
- Story formatting support (`**bold**`, `_italic_`, `==accent==`)
- Draggable left editor panel width
- High-resolution PNG export via `html2canvas`

---

## Quick Start

1. Open `posterMaker.html` in your browser.
2. Edit content in the left panel tabs:
   - **Vehicle**
   - **Specs**
   - **Story**
   - **Timeline**
   - **Colors**
3. Click **Download PNG** to export your poster.

No build process or install is required.

---

## Editor Tabs

### Vehicle
- Set poster dimensions (preset or custom width/height in inches)
- Edit title, subtitle, origin banner, and footer text

### Specs
- Add/remove/reorder **sections**
- Rename section titles
- Add/remove/reorder rows within each section
- Toggle whether empty values show em dashes
- Toggle each row value between **Normal** and **Accent**

### Story
- Add/remove paragraphs
- Inline formatting:
  - `**bold**`
  - `_italic_`
  - `==accent==`

### Timeline
- Add/remove timeline events
- Edit year and description
- Set timeline section title

### Colors
- Pick custom colors for background, header/footer, banner, labels, values, etc.
- Accent color drives decorative accents and highlight states
- Text rendering uses readability-aware color behavior

---

## Resizable Layout

The editor panel (left side) can be resized by dragging the vertical divider between the editor and preview.

---

## Export

- Use **Download PNG** to render and save a high-resolution image.
- Filename includes nickname/title and selected poster dimensions.

---

## Notes

- This app is intentionally self-contained in one HTML file.
- Uses CDN-hosted dependencies:
  - Google Fonts
  - `html2canvas`

---

## Troubleshooting

- If style changes don’t appear, do a hard refresh.
- If PNG export fails, retry once after the preview fully updates.
- Very large custom aspect ratios may require more browser memory during export.
