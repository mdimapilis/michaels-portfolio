# Michael's Portfolio — Agent Instructions

## Project Overview

**Type**: Static portfolio website  
**Hosting**: GitHub Pages (`https://mdimapilis.github.io/michaels-portfolio/`)  
**Build**: No build step — open `index.html` in a browser to preview

This is a single-page portfolio showcasing Michael's Computer Engineering background, projects, and experience. The site uses semantic HTML and a simple CSS variable system for styling.

## Key Files

- **`index.html`** — Portfolio content structure (semantic HTML with sections for education, experience, projects, skills)
- **`styles.css`** — All styling; uses CSS custom properties (`--text`, `--accent`, `--line`, etc.) for theming
- **`README.md`** — Project overview and local preview instructions

## Conventions

### HTML
- Use semantic elements (`<header>`, `<main>`, `<section>`, `<article>`)
- Include `aria-label` and `aria-labelledby` for accessibility
- External images/links (GitHub avatar, email, LinkedIn)

### CSS
- CSS variables defined in `:root` for consistent theming
- Responsive design using `min()` and CSS Grid
- Mobile-first approach with container-based sizing
- Utility classes for layout sections (`.page`, `.section`, `.item`)

### Content Structure
- Sections: Intro → Education → Experience → Projects → Skills
- Each section follows `.section` container pattern with `<h2>` headings
- Consistent spacing and typography hierarchy

## Common Tasks

| Task | Approach |
|------|----------|
| Update portfolio content | Edit `index.html` sections; content updates are live on GitHub Pages after push |
| Add/modify sections | Follow existing `.section` + `.item` pattern in HTML; update corresponding styles in `styles.css` |
| Change colors/theme | Update CSS variables in `styles.css` `:root` (e.g., `--text`, `--accent`, `--line`, `--surface`) |
| Adjust spacing | Modify CSS gap/padding values in relevant selectors (`.page`, `.section`, `.item`, etc.) |
| Preview locally | Open `index.html` in browser; no server or build required |

## Tips for AI Agents

- All styling is in one `styles.css` file — changes are isolated and easy to test
- Content lives in `index.html` — updates are straightforward HTML edits
- CSS variables make theming changes quick; avoid inline styles
- Keep the semantic HTML structure intact for accessibility and SEO
- Test responsive behavior at common breakpoints (mobile, tablet, desktop)
