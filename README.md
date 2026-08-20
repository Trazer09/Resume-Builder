

# HTML to Single-Page PDF Resume Generator

A clean, modern, and developer-friendly resume template engineered to render a pixel-perfect, ATS-compliant, single-page PDF using semantic HTML/CSS and [WeasyPrint](https://weasyprint.org/).

---

## Features

- **Strict Single-Page Layout:** Perfectly proportioned margins, line heights, and padding configured to fit standard A4 paper without awkward second-page overflow.
- **ATS-Friendly Structure:** Built using semantic HTML tags (`<h1>`, `<div class="entry">`, `<ul>`) and standard web fonts for optimal parsing across Applicant Tracking Systems.
- **Clickable Hyperlinks:** Integrated links for emails, GitHub repositories, live demo URLs, and credential certificates.
- **No External Layout Frameworks:** Written in pure HTML and vanilla CSS with no heavy JavaScript dependencies.
- **Automated PDF Compilation:** Includes a Python script utilizing WeasyPrint to instantly render `.html` into a vector `.pdf`.

---


## Quick Start (No Installation Needed)

1. Download or copy `resume.html`.
2. Open it in your favorite text editor (VS Code, Notepad, etc.) and update your information.
3. Double-click `resume.html` to open it in your browser (Chrome, Edge, Brave, Firefox).
4. Press `Ctrl + P` (or `Cmd + P` on Mac) and choose **Save as PDF**.
   - **Margins:** Set to *None* (margins are handled in CSS)
   - **Options:** Enable *Background graphics*




---

## Customization Guide

### Adjusting Spacing & Density

If your content runs onto a second page or you want to expand sections, adjust the CSS values in `<style>`:

* **Page Margins:** Change `@page { margin: 8mm 12mm; }` to increase or decrease printable area.
* **Section Gap:** Adjust `.section { margin-bottom: 6px; }` to add or reduce breathing room between headers.
* **Font Scaling:** The default base size is `8.5pt` with a `1.28` line-height. Adjust `.bullets li` or `.entry-title-left` for granular density control.

---

## License

This project is licensed under the [MIT License](https://github.com/Trazer09/Resume-Builder/blob/main/LICENSE) — feel free to fork, customize, and use it for your personal career applications.

```

```
