

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

## Project Structure

```text
├── resume.html          # Clean HTML/CSS resume template
└── README.md            # Documentation & setup instructions

```


## Quick Start (No Installation Needed)

You do **not** need to install Python or any dependencies to use this template.

1. Download or copy `resume.html`.
2. Open it in your favorite text editor (VS Code, Notepad, etc.) and update your information.
3. Double-click `resume.html` to open it in your browser (Chrome, Edge, Brave, Firefox).
4. Press `Ctrl + P` (or `Cmd + P` on Mac) and choose **Save as PDF**.
   - **Margins:** Set to *None* (margins are handled in CSS)
   - **Options:** Enable *Background graphics*

---

## Automated CLI Build (Optional for Developers)

If you prefer compiling your resume via terminal/scripts or CI/CD pipelines:

```bash
# 1. Install dependencies
pip install weasyprint

# 2. Run the generator
python generate_resume.py

```


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
