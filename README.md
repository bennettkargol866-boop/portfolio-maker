# ECTS Career Portfolio Creator

A framework-free first version of a student career portfolio builder for the ECTS Programming program.

## Run locally

Open `index.html` in a modern browser. No build step or server is required. For the smoothest browser behavior, serve the folder with any static server (for example, VS Code Live Server).

## Put it online

This is a static site and can be deployed directly to GitHub Pages, Netlify, Vercel, or any ordinary web host. Upload `index.html`, `style.css`, `script.js`, and `README.md` together; no build command or environment variables are required. Use HTTPS in production, especially if file storage is later moved to a backend.

## Included

- Guided setup and fake Demo Portfolio
- ECTS program selector covering 20 supplied pathways, including official program links
- Clear pathway outcomes: college credit, industry certification, and employment opportunities
- Board presentation mode with fictional sample data and outcome metrics
- About Me editor, repeatable work samples, accomplishments, credentials, recommendations, CareerSafe, supporting academics, and CEW Standards evidence
- Checklist and automatic required-section progress
- One canonical `Portfolio` object drives editing, checklist progress, preview, and export
- Local browser persistence with save status and reset confirmation
- Local file-name recording with a 5 MB client-side size check
- Theme and accent controls
- Live portfolio preview and browser print / Save as PDF fallback
- Responsive mobile navigation and print stylesheet

## Privacy and limitations

Version 1 stores the canonical portfolio object and file metadata in `localStorage`; it does not upload personal information or files to a server. The schema includes stable ids, nested documents, structured work samples, credentials, recommendations, CareerSafe objects, supporting academics, CEW evidence, settings, custom sections, and metadata. Because browser storage is limited and can be cleared, students should export/print their finished portfolio. A future Java backend would be needed for accounts, durable document storage, shared access, server-side PDF generation, and school-managed recovery.

The prototype records selected file names locally rather than copying file bytes into storage. The browser's print dialog is used for PDF export.
