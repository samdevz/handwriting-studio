# Assignment Generator – Handwritten Assignment Maker

**Handwriting Studio** is a browser-based handwritten-style assignment maker. Write or paste your assignment content, then format it into realistic-looking page layouts with handwriting fonts, pen styles, ink colours, and different paper options.

Use it to prepare assignment drafts, organize study notes, create printable learning materials, and preview how your typed content will look on handwritten-style pages.

> **What it does:** Handwriting Studio formats text you provide into handwritten-style pages. It does not write assignment answers from a topic or reproduce a real person's handwriting. Generated pages are simulated visuals, not genuine handwriting.

## Features

- **Handwritten assignment layout:** Turn typed assignment content into page-by-page handwritten-style previews.
- **Multiple handwriting fonts:** Choose from Caveat, Kalam, Indie Flower, Patrick Hand, Reenie Beanie, Nanum Pen Script, Shadows Into Light, Homemade Apple, Covered By Your Grace, Gloria Hallelujah, and Architects Daughter.
- **Pen and ink customization:** Select ballpoint, gel, fountain-pen, or pencil-like styling and choose an ink colour.
- **Writing adjustments:** Customize letter size, word spacing, letter spacing, and line spacing.
- **Page variation controls:** Adjust wobble, tilt, uneven spacing, occasional cross-outs, and variation down the page.
- **Assignment-friendly paper formats:** Choose A4, Letter, or A5 pages with ruled, grid, dotted, or plain layouts, plus white, cream, or legal-pad colours.
- **Assignment structure:** Add headings, subheadings, bullet points, question prompts, blank lines, and manual page breaks.
- **Page details:** Add a name, roll number, subject, date, and optional page numbers.
- **Live page preview:** View pages in list, grid, single-page, or two-page layouts; zoom in and edit a line directly on the preview.
- **Export options:** The interface includes PDF, PNG, JPG, and plain-text export settings. See the compatibility note below for the current limitation.

## Quick start

1. Clone or download this repository.
2. Rename `Handwriting Studio.html` to `index.html` (recommended for GitHub Pages).
3. Open `index.html` in a modern browser.
4. Paste or type your assignment content in the **Text** tab.
5. Add a page-one header, such as your name, roll number, and subject.
6. Choose handwriting, pen, human-variation, and page settings.
7. Review and edit the generated page previews.

No framework, build step, or application server is required for the current single-page version.

## Who may find Handwriting Studio useful?

Handwriting Studio is a general-purpose assignment formatting tool for students who want to turn their own typed drafts into handwritten-style page previews. It may be useful to learners at universities and colleges in India and internationally, including students following open, distance-learning, online, and campus-based programmes.

The following are **real institutions and illustrative examples of the wider student audience**, not customers, partners, sponsors, or endorsers of this project. Institution names are included for context and discoverability only.

### India — with a Delhi focus

- [Indira Gandhi National Open University (IGNOU)](https://www.ignou.ac.in/) — India
- [University of Delhi](https://www.du.ac.in/) — Delhi
- [Jamia Millia Islamia](https://www.jmi.ac.in/) — Delhi
- [Guru Gobind Singh Indraprastha University (GGSIPU)](https://www.ipu.ac.in/) — Delhi
- [Delhi Technological University (DTU)](https://www.dtu.ac.in/) — Delhi
- [Dr. B. R. Ambedkar University Delhi](https://aud.delhi.gov.in/) — Delhi
- [Jamia Hamdard](https://www.jamiahamdard.edu/) — Delhi
- [University of Mumbai](https://www.mu.ac.in/) — Maharashtra
- [Anna University](https://www.annauniv.edu/) — Tamil Nadu
- [University of Calcutta](https://www.caluniv.ac.in/) — West Bengal

### International examples

- [The Open University](https://www.open.ac.uk/) — United Kingdom
- [Athabasca University](https://www.athabascau.ca/) — Canada
- [University of the People](https://www.uopeople.edu/) — United States
- [Southern New Hampshire University](https://www.snhu.edu/) — United States
- [Walden University](https://www.waldenu.edu/) — United States
- [University of Nairobi](https://www.uonbi.ac.ke/) — Kenya
- [University of the Philippines Open University](https://www.upou.edu.ph/) — Philippines
- [University of Colombo](https://cmb.ac.lk/) — Sri Lanka
- [The Open University of Sri Lanka](https://ou.ac.lk/) — Sri Lanka

**Important:** These institutions are examples of potential student audiences only. Handwriting Studio is not affiliated with any institution listed above and does not provide official university templates or guarantee compliance with a particular university's assignment rules. Requirements vary by course, department, instructor, and submission type. Always check the current instructions from your own institution before preparing or submitting an assignment.

## Text formatting for assignments

Use these simple markers in the text area to structure your assignment:

| Input | Result |
| --- | --- |
| `# Assignment 1` | Large page heading |
| `## Introduction` | Smaller section heading |
| `- First point` | Bullet point |
| `Q1. Explain the topic. (5 marks)` | Question line with extra space reserved for the answer |
| `---` or `[page]` | Start a new page |
| Blank line | Preserve a blank line |

### Example assignment

```text
# Operating Systems – Assignment 1

Name: Student Name
Subject: Operating Systems

## Q1. What is an operating system? (5 marks)
An operating system is system software that manages computer hardware and provides services for applications.

## Q2. Explain the main functions of an operating system. (10 marks)
- Process management
- Memory management
- File management
- Device management

---

## Conclusion
An operating system provides the environment needed to run programs and manage computer resources.
```

The app reserves additional room below question lines based on the marks shown. You can also adjust the minimum number of lines needed before a question starts.

## Export compatibility note

The current export controls use the `claude.use('downloads')` download interface. The built-in PDF, PNG, JPG, and TXT export workflow therefore requires an environment that provides this interface. In a regular standalone browser, the app displays an export-unavailable message. Individual preview pages can still be saved as images using the browser's right-click or long-press menu.

A useful next step is to replace this environment-specific download integration with standard browser downloads so export works on normal hosting platforms, including GitHub Pages.

## Built with

- HTML
- CSS
- Vanilla JavaScript
- HTML Canvas API
- Google Fonts

The handwriting fonts are requested from Google Fonts, so an internet connection is needed to load them unless the fonts are later self-hosted.

## Privacy and storage

The current version has no application backend or upload endpoint. It stores the text and interface settings in the browser's `localStorage` under the key `hwstudio2`. The app source does not send assignment text to a server; font resources are requested from Google Fonts.

Avoid entering sensitive or confidential information on a shared device, because text can remain in that browser's local storage until it is cleared.

## Roadmap

- [ ] Add browser-native PDF, PNG, JPG, and TXT downloads.
- [ ] Add a print-friendly assignment mode.
- [ ] Add import and export for user presets.
- [ ] Improve mobile editing and page navigation.
- [ ] Add an option to self-host the font files, subject to their individual font licences.
- [ ] Add reusable assignment templates, such as title page, index, sections, and conclusion layouts.

## Responsible use

Use this tool to format your own assignment drafts, study notes, and learning materials. It creates simulated handwriting-style visuals; it does not make typed content genuinely handwritten. Follow your school or institution's rules, especially when an assignment specifically requires work to be handwritten. Do not use it to forge signatures, imitate another person's handwriting, falsify records, or misrepresent a simulated page as an authentic handwritten original.

## License

This repository is configured for the **GNU General Public License v3.0 (GPL-3.0)**. Fonts loaded from Google Fonts are separate works and remain subject to their respective font licences.
