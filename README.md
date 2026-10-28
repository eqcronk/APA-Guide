# APA-Guide

A lightweight, fully responsive, single-file web utility designed to help students and researchers navigate American Psychological Association (**APA 7th Edition**) formatting rules, generate compliant document components, and export polished files in `.docx` and `.PDF` formats.

Originally adapted from an SBL (Society of Biblical Literature) utility, this application provides an all-in-one suite for formatting student papers, title pages, reference lists, and structural headings according to official APA 7 standards.

---

## Features

1. **Interactive APA 7 Student Title Page Creator**
   - Real-time preview canvas adhering to APA 7 student title page guidelines (Title in bold, author name, department, institution, course code, instructor, and due date).
   - Instant export options to Microsoft Word (`.docx`), PDF (`.pdf`), or plain-text clipboard copy.

2. **Paper Body & Heading Generator**
   - Automatically paginates and formats body paragraphs with standard 0.5-inch paragraph indentations.
   - Supports APA 7 heading hierarchies (Level 1 Centered/Bold, Level 2 Flush-Left/Bold, Level 3 Flush-Left/Bold-Italic).
   - Auto-generates dynamic page numbers starting from Page 2.

3. **References Alphabetizer & Formatter**
   - Automatically sorts reference entries alphabetically by author last name.
   - Renders standard APA hanging indents (`0.3in`) in real-time preview canvases.

4. **Abbreviations & Acronyms List**
   - Organizes custom term definitions and academic abbreviations in a clean two-column format.

5. **Table of Contents Generator**
   - Generates dotted-leader navigation lines matching multi-level paper headings and page numbers.

6. **Built-In Citation Helper & Mistakes Guide**
   - Interactive iframe integration for quick reference lookups.
   - Comprehensive diagnostic checklist of common APA 7 errors (e.g., handling DOIs, student paper running heads, sentence-case book titles, and *et al.* rules).

---

## Tech Stack

- **HTML5 / CSS3**: Single-file architecture utilizing CSS variables, responsive flexbox layouts, and simulated print canvases.
- **Vanilla JavaScript**: Zero heavy framework dependencies; handles live DOM updates, dynamic multi-page pagination engines, and input state monitoring.
- **Client-Side Export Libraries**:
  - [`docx@8.5.0`](https://github.com/dolanmiu/docx): For generating native Microsoft Word documents entirely in the browser.
  - [`html2canvas` & `jsPDF`](https://artskydj.github.io/jsPDF/): For capturing canvas previews and compiling multi-page student papers into downloadable `.pdf` files.

---

## Getting Started

Because this utility is built entirely in a **single HTML file**, getting it running locally requires zero build tools or package managers:

1. Clone or download this repository.
2. Save the code as `index.html`.
3. Double-click `index.html` to open it directly in any modern web browser (Chrome, Firefox, Safari, Edge).

*Note: Internet connection is required on first load to fetch the CDN scripts (`docx`, `html2canvas`, `jsPDF`) and Google Fonts (`Times New Roman`).*

---

## Usage Guide

- **Switching Tabs**: Use the sticky navigation bar at the top to toggle between **Home**, **Templates**, **Format My Paper**, **Cite a Source**, and **Common Mistakes**.
- **Live Previewing**: Type or paste content into any sidebar input field. The document preview canvases on the right will update in real time.
- **Exporting**: Click any of the action buttons at the bottom of the toolbars to download your customized component as a `.docx` file, a `.pdf` file, or copy it directly to your clipboard.

---

## License

This project is open-source and available under the [MIT License](LICENSE). Feel free to adapt, modify, and use it for academic and personal projects.
