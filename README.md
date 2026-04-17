# COSHH Assessment Form

A single-file, browser-based tool for completing **Control of Substances Hazardous to Health (COSHH)** assessments in compliance with the Control of Substances Hazardous to Health Regulations 2002.

Developed at **Bangor University**.

**Live tool:** https://pjohnthomas-cpu.github.io/coshh/

## Features

- **PubChem integration** — look up GHS classification, hazard statements, and pictograms by substance name or CAS number
- **EH40 Workplace Exposure Limits** — local lookup against the UK EH40 database (bundled as `eh40.json`)
- **Multiple export formats** — PDF, Word (.docx), and ODT
- **Draft management** — save and load drafts as JSON files, or persist drafts in the browser via localStorage
- **Autosave** — automatic draft saving to browser storage while you work
- **Chemistry notation toolbar** — insert subscripts, superscripts, Greek letters, and special characters into any text field
- **Responsive design** — works on desktop, tablet, and mobile

## Usage

The tool runs entirely in the browser — no server, no installation, no account required.

1. Open `index.html` in any modern browser, or visit the live deployment
2. Fill in the assessment details, substances, controls, and emergency procedures
3. Use the **PubChem lookup** button to retrieve hazard data for each substance
4. Export the completed assessment using the format of your choice

## Files

| File | Description |
|------|-------------|
| `index.html` | The complete COSHH assessment application (self-contained) |
| `eh40.json` | EH40 Workplace Exposure Limits database (HSE, 4th edition) |
| `.nojekyll` | Prevents GitHub Pages from running Jekyll processing |

## Dependencies

All runtime dependencies are loaded from public CDNs and require an internet connection:

- [jsPDF](https://github.com/parallax/jsPDF) — PDF generation
- [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) — table support for PDF export
- [JSZip](https://stuk.github.io/jszip/) — archive support
- [docx](https://github.com/dolanmiu/docx) — Word document generation
- [IBM Plex fonts](https://fonts.google.com/specimen/IBM+Plex+Sans) — via Google Fonts

## Regulatory Context

This tool is designed to support compliance with:

- Control of Substances Hazardous to Health Regulations 2002 (COSHH)
- HSE EH40/2005 Workplace Exposure Limits (4th edition, 2020)

It is provided as a documentation aid. Completed assessments should be reviewed by a suitably qualified person before work commences.

## Author

**Dr. John Thomas Prabhakar**  
Bangor University

## Licence

MIT Licence — free to use, adapt, and redistribute with attribution.
