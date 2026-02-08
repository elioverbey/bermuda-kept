# Bermuda Kept — Jekyll Site

A membership-only Bermuda grass lawn care website for Garner, NC. Operated by Sambar LLC.

## Quick Start

```bash
# Install dependencies
bundle install

# Run locally
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

The site will be available at `http://localhost:4000`.

## Structure

```
├── _config.yml          # Site configuration & business info
├── _layouts/            # Page templates
│   ├── default.html     # Base layout with SEO schema
│   └── service.html     # Individual service page layout
├── _includes/           # Reusable components
│   ├── header.html      # Navigation header
│   └── footer.html      # Footer with NAP info
├── _services/           # Individual service pages (Markdown)
├── assets/css/          # Stylesheets
├── index.html           # Homepage
├── services/index.html  # Services overview
├── service-area.html    # Service area page (local SEO)
├── faq.html             # FAQ with schema markup
├── about.html           # About page
└── robots.txt           # Search engine directives
```

## Configuration

Edit `_config.yml` to update:
- Business name, email, address
- Typeform waitlist URL
- Site URL (update before deploying)

## Typeform Waitlist

The waitlist CTA buttons link to: `https://bermudakept.typeform.com/waitlist`

Create a Typeform with these suggested fields:
1. Full name
2. Email address
3. Property address
4. Estimated lawn square footage
5. Current grass type (confirm Bermuda)
6. How did you hear about us?
7. Anything else we should know?

## SEO Features

- JSON-LD LocalBusiness schema on every page
- JSON-LD Service schema on service pages
- JSON-LD FAQPage schema on FAQ page
- Open Graph meta tags
- Canonical URLs
- XML Sitemap (via jekyll-sitemap plugin)
- robots.txt
- Consistent NAP (Name, Address, Phone) in footer

## Cookie-Free

This site uses:
- No analytics cookies (no Google Analytics)
- No tracking scripts
- No embedded Google Maps
- Google Fonts loaded via CSS (no cookie set)
- Typeform opens in new tab (external)

No cookie consent banner needed.

## Deployment

Recommended: Deploy to Netlify, Vercel, or GitHub Pages.

For Netlify, add a `netlify.toml`:
```toml
[build]
  command = "jekyll build"
  publish = "_site"
```

## Post-Launch Checklist

- [ ] Set up Google Business Profile for "Bermuda Kept"
- [ ] Submit sitemap to Google Search Console
- [ ] Create Typeform waitlist form
- [ ] Update Typeform URL in _config.yml
- [ ] Register bermudakept.com domain
- [ ] Set up email forwarding for elioverbey@gmail.com
- [ ] List on Yelp, Angi, Nextdoor for NAP consistency
