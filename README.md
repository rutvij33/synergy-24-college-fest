# ⚡ SYNERGY '24 — Multi-Page College Fest Website

A modern, responsive, and accessible multi-page website built for **SYNERGY '24**, the premier annual college festival. Built with semantic HTML5, Vanilla CSS, and JavaScript.

---

## 🚀 Live Demo & Repository
- **Local Access:** Open `index.html` directly in any web browser, or serve via `npx serve` / `python3 -m http.server`.
- **Pages Included:**
  1. [`index.html`](index.html) — **Home Page**: Hero section, statistics, event highlights, countdown teaser, image slider, and sponsor strip.
  2. [`schedule.html`](schedule.html) — **Schedule & Timetable Page**: Day 1, Day 2, and Day 3 full event timetables with interactive day filtering, `colspan`, `rowspan`, and a print-friendly view.
  3. [`gallery.html`](gallery.html) — **Gallery & Media Page**: Interactive category photo filtering, modal lightbox, HTML5 `<video controls>`, HTML5 `<audio controls>`, YouTube promo embed (`<iframe>`), and Google Maps campus locator (`<iframe>`).
  4. [`contact.html`](contact.html) — **Registration & Contact Page**: Complete event registration form featuring 9 input types, custom real-time JavaScript validation with error messages, step-by-step progress indicator, interactive FAQ accordion, and campus contact details.
  5. [`style.css`](style.css) — **Shared Stylesheet**: Unified design system with CSS custom properties (variables), responsive Flexbox/Grid layouts, glassmorphism, micro-animations, light/dark themes, and `@media print` rules.

---

## 📋 Assignment Checklist & Rubric Compliance

### 1. Multi-Page Structure
- [x] **At least 4 pages**: `index.html`, `schedule.html`, `gallery.html`, `contact.html`.
- [x] **Consistent Navigation**: Persistent header bar on every page with active link styling for the current page and mobile hamburger drawer.
- [x] **Shared Stylesheet**: Single external `style.css` stylesheet shared across all pages.
- [x] **Consistent Footer**: Informative footer across every page with quick links, categories, and social icons.

### 2. Semantic HTML5 Tags
- [x] `<header role="banner">` on all pages for headers and hero sections.
- [x] `<nav role="navigation">` for primary navigation and mobile drawers.
- [x] `<main>` wrapping the primary page contents.
- [x] `<section>` for logical content blocks (highlights, tables, media, form).
- [x] `<article>` for cards, event previews, guidelines, and FAQ accordion items.
- [x] `<footer role="contentinfo">` on all pages.

### 3. Timetable & HTML Table Requirements
- [x] Comprehensive event timetable with `<thead>`, `<tbody>`, and semantic `<th scope="col">` headers.
- [x] Over 20 rows of events across 3 fest days (well exceeding the 6-row minimum).
- [x] **`colspan` usage**: Used in Day 1 table (`colspan="2"` for free entry) and Day 3 table (`colspan="2"` for special feature events).
- [x] **`rowspan` usage**: Used in Day 2 table (`rowspan="2"` for full-day HackFest 24 codeathon and Tech Innovation Hub venue).

### 4. Registration Form & Input Types
- [x] Form containing **9 different input types** (exceeding the 6-type requirement):
  1. `type="text"` (First Name, Last Name, College)
  2. `type="email"` (Email address)
  3. `type="tel"` (Phone number)
  4. `type="date"` (Preferred attendance date with `min` and `max` constraints)
  5. `type="number"` (Ticket quantity with `min="1"` and `max="10"`)
  6. `<select>` dropdown (Year of study)
  7. `type="radio"` (Pass type selection: Day Pass, Full Fest Pass, VIP)
  8. `type="checkbox"` (Event categories and Terms agreement)
  9. `<textarea>` (Special requirements & questions with live character counter)
- [x] Dedicated `<label for="...">` associated with every form input.
- [x] Native HTML5 validation attributes (`required`, `pattern`, `min`, `max`, `minlength`, `maxlength`).

### 5. Media & Embeds
- [x] **6+ High-Resolution Images**: Each with descriptive, meaningful `alt` text.
- [x] **HTML5 `<video controls>`**: Festival reel with playback controls and poster image.
- [x] **HTML5 `<audio controls>`**: Official fest anthem and opening percussion audio players.
- [x] **`<iframe>` Embeds**: YouTube promo teaser and embedded interactive Google Map.

### 6. Responsive Layout
- [x] Built using modern **CSS Grid** and **Flexbox**.
- [x] Responsive breakpoints at `768px` (tablets/mobile) and `480px` (smartphones).

---

## 🌟 Extra Features Implemented

1. **Dark / Light Mode Toggle (Compulsory)**:
   - Floating toggle switch (`🌙` / `☀️`) available in the navigation bar.
   - Remembers the user's choice across all pages and visits using browser `localStorage`.
2. **Mobile Hamburger Menu**:
   - Smooth slide-out mobile drawer with animated toggle button and auto-close on selection.
3. **Live JavaScript Validation**:
   - Custom, instantaneous validation on field blur and input with inline error messages below each input field.
4. **Interactive Lightbox Modal**:
   - Click any gallery image to view in a high-resolution modal popup; close via button, backdrop click, or ESC key.
5. **Interactive Photo & Schedule Filtering**:
   - Filter gallery images by category (Music, Tech, Art, Dance).
   - Filter schedule timetable by day (Day 1, Day 2, Day 3, All Days).
6. **Animated Image Carousel / Slider**:
   - Home page slider with autoplay, manual prev/next navigation, and pagination dots.
7. **Print-Friendly Timetable Layout**:
   - Dedicated `@media print` CSS rules and a "🖨️ Print Schedule" button that formats the timetable cleanly for print or PDF export.
8. **Floating "Back to Top" Button**:
   - Smooth-scrolling back-to-top button that appears after scrolling down.

---

## 🛠️ How to View Locally
Simply double click `index.html` to open it in your default web browser, or run any static server:
```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx serve
```
Then visit `http://localhost:8000` or `http://localhost:3000`.
