# Booki

Booki is a customizable booking and appointment management solution built for appointment-based businesses (barbers, salons, clinics, gyms, coaches, car services, and similar businesses).

This repository contains the product landing page (one-page website) used to present Booki and convert visitors into demo requests.

## Product Positioning

Booki is not a marketplace and not a generic SaaS template.

It is a deployable, customizable booking system installed and configured per client:

- Booking page for customers
- Admin dashboard for business owners
- Mobile-friendly interface
- Custom branding and adaptation per business

Main promise:

`Let your clients book you online.`

## Target Market

- Initial market: Algeria
- Expansion target: international / emerging markets
- Primary businesses:
  - Barbers & salons
  - Clinics / medical practices
  - Gyms / fitness
  - Trainers / coaches
  - Car services / car wash
  - Other appointment-based businesses

## What This Website Includes

The current landing page (`index.html`) includes:

- Hero section with localized messaging
- Problem / pain-point section
- How-it-works section
- Feature showcase
- Industry-specific previews
- Contact / demo request form
- Multilingual support:
  - French (`FR`)
  - English (`EN`)
  - Arabic (`العربية`) with RTL support
- Mobile off-canvas navigation (hamburger menu)
- Responsive layouts for mobile, tablet, and desktop
- Lucide icons

## Localization

The page uses a lightweight client-side i18n system (vanilla JavaScript) to switch languages dynamically.

Current localization work includes:

- `FR` as default language
- `AR` support with RTL layout adjustments
- `EN` support for international presentation
- Localized form labels and placeholders
- Algerian-friendly vocabulary (`Wilaya`, `DA`, WhatsApp-first CTA patterns)

Reference document:

- `language.md` (localization strategy)

## Tech Stack

- HTML5
- Tailwind CSS (CDN runtime for now)
- Vanilla JavaScript
- Lucide icons (CDN)

## Project Structure

```text
.
├── index.html          # Main landing page
├── context.md          # Product strategy / positioning context
├── language.md         # Localization strategy (FR/AR)
├── assets/
│   ├── hero-img.png
│   └── logo/
│       ├── logo.png
│       └── mini-logo.png
└── README.md
```

## Run Locally

This is a static site. You can run it with any local web server.

Option 1: Python

```bash
python3 -m http.server 8000
```

Then open:

`http://localhost:8000`

Option 2: Open directly

You can open `index.html` directly in the browser, but a local server is recommended for more reliable asset loading and testing.

## Production Notes

Current implementation is production-leaning, but for a stronger production setup you should consider:

- Replacing Tailwind CDN runtime with a prebuilt CSS bundle
- Replacing placeholder links (`#`) with real WhatsApp / legal links
- Wiring the demo form to a backend endpoint
- Adding analytics and event tracking (CTA clicks, form submits)
- Adding performance optimization (image compression / preload strategy)

## Design / UX Highlights

- Professional, clear visual language aligned with local SMB expectations
- Mobile-first CTA flow
- Off-canvas mobile navigation instead of dropdown menu
- Arabic RTL layout fixes for nav/hero/forms
- Horizontal scroll cards for industry previews on phone

## Developers

- Abdou Frigaa 
- Mehdi Silem — <https://github.com/MehdiSilem>

## License

No license file is currently included in this repository.
Add a `LICENSE` file before public distribution if needed.
