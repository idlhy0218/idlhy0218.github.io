# Agent Rules for idlhy0218.github.io

## 🚨 CRITICAL RULE - NEVER VIOLATE THIS

### **NEVER Change File Paths in HTML Code**

**This is the most important rule. When editing ANY HTML file in this project:**

- **DO NOT** modify any file paths that reference GitHub repository structure unless performing an explicit file rename operation requested by the user.
- **DO NOT** change relative paths like `../page building/`, `../images/`, etc.
- **DO NOT** "fix" or "optimize" paths that look redundant (e.g., `../page building/blog/` is intentional)
- **DO NOT** convert relative paths to absolute paths or vice versa
- **DO NOT** reorganize folder structure without explicit user permission

**Why this matters:** GitHub Pages has a specific deployment structure. Changing paths will break the live website even if it works locally.

---

## 🎨 Design System: Light Gallery Theme

All new and modified pages in this project must follow the **Light Gallery** aesthetic:

### 1. Color Palette
- **Canvas/Background**: `#fbfbfa` (Elegant warm gallery off-white)
- **Vignette Background**: Fixed `.ambient-overlay` (radial gradient transitioning to soft dark slate)
- **Primary Text**: `#111827` (Solid charcoal black)
- **Secondary Text**: `#575757` (Sophisticated dark slate gray)
- **Accent Color**: Terracotta Orange `#ea580c` (derived from network nodes, used for years, headers, and section accents)
- **Link Highlight**: Electric Blue `#2563eb` (used for inline hyperlinks, DOI tags, and interactive hover states)

### 2. Typography
- **UI & Headers**: `'Outfit', sans-serif` (used for page titles, course headers, publication years, dates, and buttons)
- **Paragraph Body & Quotes**: `'Inter', sans-serif` (used for descriptions, student comments, and bibliography listings)

### 3. Layout Philosophy
- **Whitespace & Breathing Room**: Prioritize generous margin padding over dense grid lines.
- **No Card Boxes**: Avoid enclosing text in cards, boxes, backgrounds, borders, or dropshadows. Let the typography sit naturally on the warm-white canvas.
- **Thin Separators**: Use thin slate borders or dashed lines (`rgba(15, 23, 42, 0.08)`) to structure sections.

---

## General Development Rules

### Navigation Structure
- The site navigation consists of 6 primary items:
  1. **Publications** (`publications.html`)
  2. **Teaching** (`teaching.html`)
  3. **Stats Lab** (`statslab.html`)
  4. **Gallery** (`gallery.html`)
  5. **CV** (`cv.html`)
  6. **Contact** (`contact.html`)
- **About** and **Blog** pages/tabs are completely deleted.
- Navbars should remain floating glass containers (`backdrop-filter: blur(20px)`) centered at the top.

### Stats Lab Management
- All tutorials are listed dynamically inside `page building/statslab.html` in the `statsLabPosts` array.
- Stats Lab items do **NOT** show a "Read Article" text link at the bottom.
- Instead, the tutorial title itself must be wrapped in an anchor tag pointing directly to the `.html` post file.
- The title link must change from charcoal black to electric blue with an underline on hover.

### Gallery Management
- Gallery visual charts and maps are managed in `page building/gallery.html` in the `galleryImages` array.
- Images render in a responsive grid and open in a responsive modal lightbox when clicked.

---

## Quality Checklist

Before finalizing any changes:

- [ ] All file paths remain correct and unchanged
- [ ] No broken links or 404 errors when clicking navbar items
- [ ] Responsive design works properly on mobile viewports
- [ ] Title links in Stats Lab are clickable and hover states function correctly
- [ ] Embedded PDF viewer on CV page is responsive and fully loaded

**Last Updated:** 2026-07-18  
**Project Owner:** Heeyoung Lee  
**Repository:** idlhy0218.github.io
