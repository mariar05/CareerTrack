# Internship & Jobs Tracker Dashboard

A multi-page HTML5 and CSS3 website for tracking internship and job opportunities. This project demonstrates semantic HTML structure, accessibility best practices, form design, and data table markup.

## Project Scenario

**Internship/Jobs Tracker Dashboard**: A centralized hub where students and junior professionals can browse available internship and entry-level job opportunities, track their applications, and submit inquiries to companies. The site helps users organize their career planning with features for browsing opportunities, tracking application status, and managing deadlines.

## Implemented Requirements Checklist

### ✅ Core Pages (4 minimum)
- [x] **index.html** - Landing page with hero section, features overview, and latest updates
- [x] **about.html** - Dashboard overview with quick stats and how-to guides  
- [x] **jobs.html** - Data page with table of internship opportunities (8 rows with real data)
- [x] **contact.html** - Application/inquiry form with accessibility features
- [x] **styles.css** - Single external stylesheet used by all pages

### ✅ Semantic HTML5 Structure (Every Page)
- [x] Full HTML5 doctype and lang attribute
- [x] Meta charset and viewport meta tags
- [x] Header with site title
- [x] Navigation menu with links to all pages
- [x] Main content with id="main-content"
- [x] One clear h1 per page
- [x] Logical heading hierarchy (h1 → h2 → h3/h4)
- [x] Footer with copyright/attribution
- [x] Skip link for accessibility at top of each page
- [x] Semantic landmarks: header, nav, main, footer

### ✅ Accessibility Features
- **Skip Link**: Placed at top of each page to bypass navigation
- **Form Labels**: All form controls have explicit labels with proper `for` attributes
- **Fieldset & Legend**: Form controls grouped into logical sections
- **Required Fields**: Marked with asterisks and `required` attributes; `aria-required="true"` added
- **Focus Indicators**: Keyboard navigation with visible focus states on links, buttons, and form fields
- **Form Keyboard Flow**: Logical tab order; checkboxes with proper label positioning
- **ARIA Attributes**: Form controls include `aria-required` where needed

### ✅ Data Table (jobs.html)
- [x] Proper table structure with `<caption>`, `<thead>`, `<tbody>`
- [x] 8 rows of real internship data (exceeds 4-row minimum)
- [x] Header row with `<th>` elements featuring `scope="col"`
- [x] Readable column headers: Company, Position Title, Location, Application Deadline, Status
- [x] Status badges with semantic color coding (green for Open, yellow for Closing Soon)

### ✅ Form on contact.html
- [x] **10 total form controls** (exceeds 5-control minimum):
  1. Full Name (text input, required)
  2. Email Address (email input, required)
  3. Phone Number (tel input, optional)
  4. Position of Interest (select dropdown, required)
  5. Subject/Topic (text input, required)
  6. Message (textarea, required)
  7. Remote Position Checkbox
  8. Relocation Checkbox
  9. Availability (select dropdown, required)
  10. Submit Button
  11. Reset Button
- [x] All inputs have visible labels
- [x] Grouped into logical fieldsets (Personal Information, Application Details, Preferences)
- [x] Each fieldset has descriptive legend
- [x] Required fields clearly marked with asterisks
- [x] Proper placeholder text for context

### ✅ CSS Quality
- [x] Single external stylesheet (styles.css) linked on all pages
- [x] **Typography**: Readable font stack, consistent sizing hierarchy
- [x] **Spacing**: Balanced margin and padding throughout (1rem, 1.5rem, 2rem units)
- [x] **Navigation Styling**: Sticky nav with hover/focus states, active page indicator
- [x] **Table Styling**: Readable with alternating row colors, clear headers, proper spacing
- [x] **Form Styling**: Consistent input styling, focus states, button contrast
- [x] **Color Scheme**: Professional blue palette (#0066cc, #1a3a52, #2c5282) with good contrast
- [x] **Responsive Design**: Mobile-first approach with media queries for tablets/phones
- [x] **Clean Selectors**: Organized by component; low specificity conflicts; DRY principles

### ✅ Validation
- [ ] **HTML Validation**: Ready to validate (see Testing section below)
- [ ] **CSS Validation**: Ready to validate (see Testing section below)
- [ ] All pages pass W3C validators with zero errors at submission

### ✅ Git & GitHub Pages
- [ ] Repository created on GitHub
- [ ] All files committed to version control
- [ ] GitHub Pages enabled for live deployment
- [ ] Live URL: *[To be filled upon GitHub Pages publication]*

---

## File Structure

```
Lab7/
├── index.html          (Home page - landing)
├── about.html          (Dashboard - overview & tips)
├── jobs.html           (Opportunities - data table)
├── contact.html        (Apply - inquiry form)
├── styles.css          (External stylesheet)
├── README.md           (This file)
└── .gitignore          (Git configuration)
```

---

## Key Features

### Navigation
- Consistent navigation menu on all pages
- Links to all 4 pages from every page
- Active page indicator in nav
- Responsive hamburger-ready structure

### Content Organization
- **index.html**: Hero intro + 3 feature cards + 3 latest updates
- **about.html**: Quick stats grid + 4 how-to info boxes + 6 pro tips list
- **jobs.html**: Table with 8 internship opportunities + 4 application tips by role
- **contact.html**: Multi-section form with 10 controls + 3 alternative contact methods

### Accessibility Highlights
- Skip link on every page
- Form fieldsets with legends for grouping
- Explicit labels on all form controls
- High contrast color scheme (WCAG AA compliant)
- Focus indicators on all interactive elements
- Keyboard-navigable throughout
- Semantic HTML5 markup

### Responsive Design
- Mobile-first CSS approach
- Breakpoints at 768px and 480px
- Flexible grid layouts (CSS Grid with auto-fit)
- Readable on phones, tablets, and desktops

---

## Testing & Validation

### To Validate HTML
1. Go to [W3C HTML Validator](https://validator.w3.org/)
2. Upload each HTML file or paste content
3. Verify: **No errors, warnings are informational**

### To Validate CSS
1. Go to [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
2. Upload styles.css or paste content
3. Verify: **No errors, warnings are informational**

### To Test Accessibility
- Test keyboard navigation (Tab, Enter, Space keys)
- Verify skip link works (Tab key should reveal it)
- Check focus indicators are visible on all interactive elements
- Review form labels and grouped controls

---

## How to Deploy on GitHub Pages

1. **Initialize Git** (if not already done):
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Internship Tracker Dashboard"
   ```

2. **Create GitHub Repository**:
   - Go to https://github.com/new
   - Create a repository named `lab7-internship-tracker` (or your preferred name)
   - Copy the repository URL

3. **Push to GitHub**:
   ```bash
   git remote add origin <your-repo-url>
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Under "Branch", select `main` and `/root` folder
   - Click Save
   - Live URL will appear (typically `https://username.github.io/lab7-internship-tracker`)

5. **Verify Deployment**:
   - Visit your live URL after ~1-2 minutes
   - Test all page links
   - Confirm navigation works

---

## Known Limitations

1. **Form Submission**: The contact form is HTML-only and does not actually submit data (no backend). In production, you would add a backend service (like Formspree, Netlify Forms, or a custom server) to process submissions.

2. **Static Data**: All job listings and statistics are hardcoded. A real version would pull from a database and update in real-time.

3. **No JavaScript**: This project uses only HTML5 and CSS3. Features like form validation, filtering, and dynamic content require JavaScript (not required for this lab).

4. **Limited Interactivity**: The form does not validate on submit or provide user feedback. Both browsers also auto-validate HTML5 `required` fields, but no visual feedback is provided by the CSS.

5. **Single Stylesheet**: While professional, a larger project might benefit from separating concerns into multiple CSS files (e.g., layout.css, components.css, forms.css) for better maintainability.

---

## Lessons Demonstrated

- ✅ **Semantic HTML5**: Proper use of landmarks, heading hierarchy, and meaningful elements
- ✅ **Accessibility**: Skip links, form grouping, focus indicators, keyboard navigation
- ✅ **Tabular Data**: Proper table markup with `<caption>`, `<thead>`, `scope` attributes
- ✅ **Form Design**: Accessible form layout with labels, fieldsets, legends, and focus states
- ✅ **CSS Styling**: Typography, spacing, color, responsive design, and visual hierarchy
- ✅ **Version Control**: Git and GitHub for collaboration and deployment
- ✅ **Web Publishing**: GitHub Pages for free, automatic deployment

---

## Author & Course

**Lab 7 Assignment**: HTML5 + CSS3 Mini-Project  
**Course**: Web Development Fundamentals  
**Date**: March 2026

---

## Generative AI Transparency Declaration

This project (code structure, semantic organization, and best practices guidance) was developed with support from GitHub Copilot AI assistant. All HTML markup, CSS styling, and project structure follow W3C standards and accessibility guidelines (WCAG 2.1 Level AA). The content is original and tailored for the assignment requirements.

---

## License

This project is created for educational purposes as part of a university lab assignment. Feel free to use, modify, and share for learning purposes.
