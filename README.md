# Thompson & Sons Plumbing — Website Project

## Student Information

- **Full Name:** Neo Maleka
- **Student Number:** ST10507580
- **Module:** WEDE5020 – Web Development
- **Group:** 1
- **Year:** 2026

## Project Overview

Thompson & Sons Plumbing is a small, family-run plumbing business founded in 2011 by David Thompson, serving homeowners, property managers, and small commercial clients across the greater Johannesburg area. The business has grown from a one-man operation into a team of four qualified plumbers offering installation, maintenance, and emergency repair services, but currently has no website — relying solely on a Facebook page and word-of-mouth referrals.

This project delivers a responsive, mobile-first website that gives Thompson & Sons a professional web presence, makes it easy for customers to request a quote online (including a photo of the issue), and builds trust through visible credentials, testimonials, and clear service information — reducing the business's reliance on phone-only enquiries.

## Website Goals and Objectives

- Generate qualified leads through an online enquiry and quote-request form.
- Build trust with new customers through visible testimonials, certifications, and service guarantees.
- Provide clear information on services offered and emergency contact availability.
- **KPIs:** number of quote requests per month, average time-on-site, and reduction in phone-only enquiries.

## Key Features and Functionality

- **Homepage** with a clear call-to-action for emergency callouts, a "Recent Work" photo gallery, and an overview of the business.
- **Services page** detailing installations, repairs & maintenance, and emergency callouts.
- **Online quote-request form** with a file upload for photos of the issue.
- **About Us page** featuring the company history, mission, vision, and team credentials.
- **Contact page** with a map placeholder, phone number, email, and WhatsApp click-to-chat link.
- **Sticky call-to-action** button on mobile for one-tap emergency calling.
- **Mobile-first, single-column layout** with large, tap-friendly buttons, since most enquiries are expected from customers on their phones during an emergency.

## Design and User Experience

| Element | Choice |
|---|---|
| Colour scheme | Navy blue (#0B2545) and safety orange (#FF6A2B) — conveying trust and urgency |
| Typography | Oswald (headings) paired with Open Sans (body text) |
| Layout | Single-column, mobile-first |
| Signature detail | A "pipe route" SVG divider between sections, echoing the copper pipework installed on every job |
| Wireframes | Low-fidelity wireframes for the Homepage, Services page, and Contact page are included in the Website Project Proposal document (see Part 1 Details below) |

## Timeline and Milestones

| Week | Milestone |
|---|---|
| Week 1–2 | Research, wireframing, and content gathering |
| Week 3–4 | Homepage and core page development |
| Week 5 | Forms, testing, and mobile responsiveness checks |
| Week 6 | Client review, revisions, and final submission |

## Part 1 Details

Part 1 covered the **Website Project Proposal** (including low-fidelity wireframes for the Homepage, Services page, and Contact page) and the initial **static HTML build**, consisting of:

- `index.html` — Homepage
- `about.html` — About Us
- `services.html` — Services
- `enquiries.html` — Get a Quote (enquiry form)
- `contact.html` — Contact

## Part 2 Details

Part 2 applied CSS styling to the desktop solution, built on the Part 1 HTML structure. All styling lives in the single external stylesheet, `style.css`, linked from every page.

- **External stylesheet:** one `style.css`, linked consistently across all five pages with `<link rel="stylesheet" href="style.css">`.
- **Base style:** a lightweight CSS reset (`box-sizing`, margin/padding, list and link resets) plus site-wide defaults for font family, font size, and the navy/safety-orange colour scheme.
- **Typography:** Oswald for headings and Open Sans for body copy, on a consistent `rem`-based type scale with defined `line-height` and `letter-spacing`.
- **Layout structure:** Flexbox for one-dimensional rows (header, nav, footer items, button groups) and CSS Grid for two-dimensional sections (card grids, two-column layouts, the photo gallery).
- **Visual styles:** `color`, `background-color`, `border`, and `box-shadow` style every element, with `:hover`, `:focus-visible`, and `:active` states on all buttons, nav links, and form fields.
- **Responsive design:**
  - **Breakpoints:** Desktop (≥1024px, default), Tablet (768px–1023px), Mobile (<768px) — each with its own media query.
  - **Relative units:** font sizes and spacing set in `rem`; headings use `clamp()` with `vw` for fluid scaling.
  - **Responsive images:** `img { max-width: 100%; }` site-wide, plus an `object-fit: cover` photo-container pattern (`.photo-grid` / `.photo-frame`) so photos crop neatly to a consistent shape at any screen size.
- **Testing:** styles were checked in browser DevTools at 375px (mobile), 820px (tablet), and 1440px (desktop) to confirm the layout switches from single-column to multi-column correctly at each breakpoint. Screenshot evidence of each breakpoint is included below and in the submitted proposal document.

### Screenshot Evidence (Responsive Testing)

> Add screenshots of the site at each breakpoint here before submission:
> - Desktop (1440px): `screenshots/desktop.png`
> - Tablet (820px): `screenshots/tablet.png`
> - Mobile (375px): `screenshots/mobile.png`

## Sitemap

```
Home (index.html)
├── About (about.html)
├── Services (services.html)
├── Get a Quote (enquiries.html)
└── Contact (contact.html)
```

## Technical Requirements

- **Hosting and domain:** Shared hosting package with a .co.za domain (e.g., thompsonplumbing.co.za)
- **Languages and frameworks:** HTML5, CSS3, and JavaScript, built as a responsive static site (with optional lightweight PHP contact-form handling)

## Changelog

All notable changes to this project are documented below, newest first.

### [Unreleased]
- Planned: dynamic backend for the quote-request form (Part 3)
- Planned: content management for testimonials and service pricing (Part 3)

### [0.4.0] — Part 2 (Responsive & Interactive Styling)
- Restructured `style.css` into clearly labelled sections matching the module brief (external stylesheet, base style, typography, layout structure, visual styles, breakpoints, relative units, responsive images, testing).
- Converted font sizes and spacing to `rem` units for accessibility and consistency; fluid headings via `clamp()`.
- Added an explicit three-tier breakpoint system: Desktop (≥1024px), Tablet (768–1023px), Mobile (<768px).
- Added `:hover`, `:focus-visible`, and `:active` interaction states to all buttons, nav links, and form fields.
- Added a CSS reset and consolidated colour variables (`:root` custom properties).

### [0.3.0] — Part 1 Feedback Edits
- Added low-fidelity wireframes (Homepage, Services page, Contact page) to the Website Project Proposal document, addressing formative feedback ("No wireframes provided — 0/2").
- Reviewed and confirmed proposed features, design aesthetic, technical requirements, timeline, and budget sections against formative feedback; no further changes required as these sections scored full marks.

### [0.2.0] — Part 1 (Services Page)
- Added `services.html` detailing Installations, Repairs & Maintenance, and Emergency Callouts.
- Updated navigation and footer links across all pages to include Services.
- Added a "Recent Work" photo gallery container (`.photo-grid` / `.photo-frame`) to the homepage, using `object-fit: cover` and `aspect-ratio` so photos of any size fit consistently.

### [0.1.0] — Part 1 (Initial Build)
- Created `index.html`, `about.html`, `contact.html`, and `enquiries.html`.
- Implemented shared `style.css` design system (navy/safety-orange palette, Oswald + Open Sans typography).
- Implemented `script.js` for mobile nav toggle, quote form submission, and photo file-upload interaction.
- Added sticky mobile call-to-action button and 24/7 emergency strip.

## References

- Krug, S. (2014). *Don't Make Me Think, Revisited: A Common Sense Approach to Web Usability*. New Berkeley: New Riders.
- MDN Web Docs. (2026). *CSS Flexible Box Layout*. Available at: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout [Accessed 2026].
- MDN Web Docs. (2026). *CSS Grid Layout*. Available at: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout [Accessed 2026].
- MDN Web Docs. (2026). *Using Media Queries*. Available at: https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries [Accessed 2026].
- W3Schools. (2026). *HTML and CSS Responsive Web Design*. Available at: https://www.w3schools.com [Accessed 2026].
