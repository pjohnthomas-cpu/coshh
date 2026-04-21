# COSHH Assessment Form

A browser-based COSHH support site with two main tools:

- A hazard profile lookup tool for researching substances against EH40, PubChem, and EPA CTX
- A full single-page COSHH assessment tool for drafting, saving, and exporting COSHH forms

Designed for broader research-laboratory use.

**Live site:** https://coshh.uk/

## Site structure

- `index.html` — landing page with preparation guidance, resource links, and entry points into the tool
- `hp.html` — hazard profile lookup tool for EH40, PubChem, and EPA CTX substance research
- `app.html` — the full COSHH assessment application
- `eh40_data.json` — bundled EH40 Workplace Exposure Limits dataset used for local lookup
- `.nojekyll` — prevents GitHub Pages from running Jekyll processing

## Tool features

- **PubChem integration** — look up GHS classification, hazard statements, and pictograms by substance name or CAS number
- **EH40 Workplace Exposure Limits** — local lookup against the bundled EH40 dataset
- **Multiple export formats** — PDF, Word (`.docx`), and ODT
- **Draft management** — save and load drafts as JSON files, or persist drafts in the browser via localStorage
- **Autosave** — automatic draft saving to browser storage while you work
- **Chemistry notation toolbar** — insert subscripts, superscripts, Greek letters, and special characters into compatible text fields
- **Responsive design** — works on desktop, tablet, and mobile

## Usage

1. Open the live site or load `index.html` in a browser
2. Review the preparation checklist and linked reference material
3. Open the tool from the landing page or go directly to `app.html`
4. Fill in the assessment details, substances, controls, and emergency procedures
5. Use the built-in lookup tools to support hazard and exposure-limit checks
6. Export the completed assessment in the format you need

## Dependencies

All runtime dependencies are loaded from public CDNs and require an internet connection:

- [jsPDF](https://github.com/parallax/jsPDF) — PDF generation
- [jsPDF-AutoTable](https://github.com/simonbengtsson/jsPDF-AutoTable) — table support for PDF export
- [JSZip](https://stuk.github.io/jszip/) — archive support
- [docx](https://github.com/dolanmiu/docx) — Word document generation
- [IBM Plex fonts](https://fonts.google.com/specimen/IBM+Plex+Sans) — via Google Fonts

## Regulatory context

This project is designed to support compliance with:

- Control of Substances Hazardous to Health Regulations 2002
- HSE EH40/2005 Workplace Exposure Limits, including later amendments reflected in the bundled dataset

It is provided as a documentation aid. Completed assessments should be reviewed by a suitably qualified person before work commences.

## Author

**Dr. John Thomas Prabhakar**  
john.thomas@bangor.ac.uk

## Licence

MIT Licence — free to use, adapt, and redistribute with attribution.
