<a name="readme-top"></a>

# edisontkpcom.github.io

Personal resume & portfolio site for Edison Tan Khai Ping. This static site hosts an interactive, theme-switchable, PDF-exportable CV highlighting experience in AI, autonomous agentic systems, blockchain (DeFAI), quantum computing exploration, cloud architecture, and full stack engineering.

Live site: https://edisontkpcom.github.io/

## Features

- Responsive two-column resume layout (desktop) collapsible navigation (mobile)
- Dark / light theme toggle (persisted with localStorage)
- Active section highlighting while scrolling
- Scroll-to-top control
- One-click PDF export (html2pdf) with automatic A4 scaling
- Structured sections: Profile Overview, Technical Skills, Experience, Education, Certifications, Training & Speaking, Awards, Portfolio, Blockchain Timeline, References

## Tech Stack

- HTML5 + CSS3 (custom, no framework)
- Vanilla JavaScript (UI interactions & PDF trigger)
- Boxicons icon set
- html2pdf.js bundle for PDF generation

## Project Structure

```
index.html          # Main resume/portfolio
index1.html         # Legacy / earlier version (kept for reference; can be removed)
assets/css/styles.css
assets/js/main.js
assets/js/html2pdf.bundle.min.js
assets/img/*        # Images & favicon
```

## Local Development

Clone the repository and open `index.html` in any modern browser:

```
git clone https://github.com/EdisonTKPcom/edisontkpcom.github.io.git
cd edisontkpcom.github.io
```

Optionally use a lightweight static server (improves PDF rendering consistency):

```
python3 -m http.server 8080
# or
npx serve .
```
Then browse to http://localhost:8080

## PDF Export Tips

- Use the desktop layout (width ≥ 968px) to enable the floating PDF icon.
- Click the download icon; scaling class is applied temporarily for an A4-friendly layout.
- If fonts appear blurry, increase `html2canvas.scale` in `assets/js/main.js` (current: 4).

## Customization

Edit content directly in `index.html`. Sections are semantically grouped; add/remove list items or blocks (`experience_content`, `certificate_content`, etc.) to extend.

Adjust colors or typography in `:root` variables inside `assets/css/styles.css`.

## Planned Enhancements

- Structured data (JSON-LD Person schema)
- Image optimization & `<picture>` responsive sources
- Optional print-specific stylesheet (reduce reliance on JS scaling)
- Lighthouse performance & accessibility refinements

## License

Content © Edison Tan Khai Ping. Source code released under MIT unless otherwise noted.

## Contact

Website: https://edisontkp.com  
LinkedIn: https://linkedin.com/in/edisontkp  
Email: im@edisontkp.com  

---
If you find this template useful, feel free to fork and adapt for your own developer resume site.
