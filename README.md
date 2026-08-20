

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
├── generate_resume.py   # Python script to compile HTML to PDF
└── README.md            # Documentation & setup instructions



---

## Prerequisites & Installation

### 1. System Dependencies (Linux / Ubuntu / Debian)

WeasyPrint requires underlying rendering and font libraries (`pango`, `cairo`, `harfbuzz`):

```bash
sudo apt update
sudo apt install -y python3-venv python3-pip libpango-1.0-0 libpangoft2-1.0-0 libharfbuzz-subset0 libffi-dev

```

*(For macOS: `brew install pango` | For Windows: Install GTK3 runtime as per WeasyPrint docs).*

### 2. Python Environment Setup

To avoid `PEP 668` conflicts with system packages, use a virtual environment:

```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
# On Linux/macOS:
source venv/bin/activate
# On Windows:
# .\venv\Scripts\activate

# Install WeasyPrint
pip install weasyprint

```

---

## Usage

### Method A: Automated Python Compilation (Recommended)

1. Clone this repository:
```bash
git clone [https://github.com/Trazer09/html-resume-generator.git](https://github.com/Trazer09/html-resume-generator.git)
cd html-resume-generator

```


2. Open `generate_resume.py` (or `resume.html`) and replace the template text with your own experience, education, and links.
3. Run the compiler:
```bash
python generate_resume.py

```


4. Find your generated PDF (`Sidhant_Kumar_Resume.pdf`) in the project directory.

---

### Method B: Browser Print-to-PDF (No Python Needed)

1. Double-click and open `resume.html` in any modern web browser (Chrome, Brave, Firefox, Edge).
2. Press `Ctrl + P` (or `Cmd + P` on macOS).
3. Set **Destination** to `Save as PDF`.
4. In **More Settings**:
* **Paper Size:** `A4`
* **Margins:** `None` (Margins are handled via CSS `@page`)
* **Options:** Check **Background graphics**


5. Click **Save**.

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
