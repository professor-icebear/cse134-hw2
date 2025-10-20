# HTML Tag Checklist for HW2

## All Required Tags (43 total) - ✓ Complete

### Demonstrated Across Main Pages

#### Document Structure Tags
- ✓ `<html>` - All pages
- ✓ `<head>` - All pages
- ✓ `<title>` - All pages
- ✓ `<meta>` - All pages (charset, viewport, description, author, keywords)
- ✓ `<link>` - All pages (favicon, CSS links)
- ✓ `<script>` - index.html (custom elements + analytics placeholder)
- ✓ `<style>` - index.html, projects.html, contact.html (border styling only)
- ✓ `<body>` - All pages

#### Semantic Structure Tags
- ✓ `<main>` - All pages
- ✓ `<header>` - All pages
- ✓ `<footer>` - All pages
- ✓ `<nav>` - All pages
- ✓ `<section>` - All pages
- ✓ `<article>` - index.html, projects.html, research.html, artwork.html

#### Heading Tags
- ✓ `<h1>` - All pages
- ✓ `<h2>` - All pages
- ✓ `<h3>` - All pages

#### Text Content Tags
- ✓ `<p>` - All pages
- ✓ `<div>` - index.html, 404.html
- ✓ `<span>` - index.html
- ✓ `<br>` - index.html, 404.html, contact.html

#### Text Formatting Tags
- ✓ `<b>` - index.html
- ✓ `<i>` - index.html
- ✓ `<strong>` - index.html, research.html
- ✓ `<em>` - index.html, research.html

#### List Tags
- ✓ `<ul>` - All pages (navigation + content lists)
- ✓ `<ol>` - projects.html, research.html, projects/mav.html, projects/tutor.html
- ✓ `<li>` - All pages

#### Link and Media Tags
- ✓ `<a>` - All pages (navigation + content links)
- ✓ `<img>` - artwork.html, experiments.html
- ✓ `<picture>` - artwork.html, experiments.html
- ✓ `<iframe>` - projects/tutor.html
- ✓ `<svg>` - artwork.html

#### Form Tags
- ✓ `<form>` - contact.html
- ✓ `<label>` - contact.html
- ✓ `<fieldset>` - contact.html
- ✓ `<legend>` - contact.html
- ✓ `<input>` - contact.html (text, email, tel, range)
- ✓ `<textarea>` - contact.html
- ✓ `<button>` - contact.html (submit, reset)

#### Other Tags
- ✓ `<progress>` - projects/mav.html
- ✓ `<dialog>` - contact.html
- ✓ `<noscript>` - index.html

### Demonstrated in experiments.html ONLY

These 6 tags are exclusively demonstrated in experiments.html:

- ✓ `<template>` - experiments.html
- ✓ `<audio>` - experiments.html  
- ✓ `<video>` - experiments.html
- ✓ `<canvas>` - experiments.html (with minimal JS demo)
- ✓ `<source>` - experiments.html (used with audio, video, picture)

Note: `<picture>` appears in both artwork.html AND experiments.html

## Custom Elements (2 required) - ✓ Complete

### 1. Semantic CSS Custom Element - ✓
- **Element Name:** `<profile-card>`
- **Location:** index.html
- **Purpose:** Semantic custom element for displaying card-style content
- **Implementation:** Defined using Web Components API
- **Styling:** Custom CSS styling applied (does not count towards 3-property limit)

### 2. Hello World Custom Element - ✓
- **Element Name:** `<hello-world>`
- **Location:** index.html
- **Purpose:** Logs "Hello World!" to the browser console
- **Implementation:** Uses connectedCallback() to print to console without modifying DOM

## CSS Usage - ✓ Within Limits

**Total CSS properties used (excluding custom element): 3**

Border properties only (allowed):
- `border: 1px solid #ccc;` in index.html (main element)
- `border: 2px solid #333;` in projects.html (section element)
- `border: 1px solid #999;` in contact.html (form element)

**Custom element styling (profile-card):** Does NOT count towards limit
- All CSS within `profile-card` selector is excluded per assignment rules

## JavaScript Usage - ✓ Within Limits

JavaScript is only used where permitted:

1. **Canvas demonstration** - 14 lines in experiments.html (under 15-line limit)
2. **Custom elements** - Web Components API for both custom elements in index.html
3. **Analytics placeholder** - Script tag for future analytics in index.html

No interactive JavaScript or DOM manipulation (except for custom elements and canvas demo as allowed).

## Pages Created (10 total)

1. ✓ **index.html** - Home page with custom elements
2. ✓ **projects.html** - Projects listing page
3. ✓ **projects/mav.html** - MAV project details
4. ✓ **projects/factify.html** - Factify project details
5. ✓ **projects/tutor.html** - Tutor platform details
6. ✓ **artwork.html** - Artwork gallery with picture and svg
7. ✓ **research.html** - Research publications
8. ✓ **contact.html** - Contact form with dialog element
9. ✓ **404.html** - Error page
10. ✓ **experiments.html** - Simplified page showing only template, picture, audio, video, canvas, source

## Tag Distribution Strategy

### experiments.html (6 tags only)
- template
- picture (with source)
- audio (with source)
- video (with source)
- canvas (with minimal JS)
- source

### Other Pages (37 remaining tags)
All other required tags are distributed semantically across:
- index.html (custom elements, noscript)
- projects.html and project detail pages (progress, ol, iframe)
- artwork.html (img, picture, svg)
- research.html (article, strong, em)
- contact.html (all form elements, dialog, button)
- 404.html (div, br)

## Directory Structure

```
/
├── index.html
├── projects.html
├── projects/
│   ├── mav.html
│   ├── factify.html
│   └── tutor.html
├── artwork.html
├── research.html
├── contact.html
├── 404.html
├── experiments.html
└── assets/
    ├── images/ (ready for your images)
    └── pdf/ (ready for your resume)
```

## Validation Checklist

Before submission:
1. ✓ All 43 tags used appropriately
2. ✓ Both custom elements implemented correctly
3. ✓ CSS usage within limits (3 properties, border only)
4. ✓ JavaScript only for allowed purposes (canvas, custom elements, analytics placeholder)
5. ✓ No "div-itis" - semantic HTML used throughout
6. ✓ experiments.html shows only the 6 required tags
7. ✓ All other tags demonstrated across remaining pages

## Next Steps

1. Add your images to `assets/images/` (artwork-1.jpg, artwork-2.png, etc.)
2. Add your resume PDF to `assets/pdf/`
3. Validate ALL pages at https://validator.w3.org/
4. Test custom elements (open browser console to see "Hello World!" message)
5. Deploy to Netlify
6. Re-validate on deployed site

## Testing Tips

- **Custom Elements:** Open index.html in browser and check console for "Hello World!" message
- **Canvas:** Check experiments.html for rendered shapes and text
- **Forms:** Verify all form controls work in contact.html
- **Navigation:** Test all navigation links work correctly
- **Validation:** Use https://validator.w3.org/ for each page

Your site is ready for validation and deployment! 🚀
