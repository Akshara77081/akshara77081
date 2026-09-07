This is a static portfolio website for Akshara Bharathi S, a Full Stack Developer / AI & Data Science student.

## Architecture
- Plain static HTML/CSS/JS — no framework, no build step.
- `index.html` — single-page site with sections for Home, About, Skills, Projects, Experience, Education, Certifications, and Contact, linked via in-page anchors.
- `style.css` — all styling, including a mobile nav flyout toggled via a `.open` class on `#nav`.
- `script.js` — sets the footer copyright year and wires up the mobile menu button (`#menuBtn`) to toggle `#nav.open`.
- `images/` — profile photo and other static assets.
- `netlify.toml` — publishes the repo root as-is (`publish = ".""`), since there is no build step.

## Conventions
- Sections are identified by id (`#home`, `#about`, `#skills`, `#projects`, `#experience`, `#education`, `#certifications`, `#contact`) and referenced directly by the nav links.
- Content (bio, projects, certifications, contact links) is hardcoded directly in `index.html`; there is no CMS or data file.

## Non-obvious decisions
- `script.js` was added because the original design referenced it (for the year and mobile menu) but the file wasn't present in the initial upload; the corresponding `nav.open` CSS already existed in `style.css`.
