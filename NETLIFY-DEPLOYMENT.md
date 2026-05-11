# PawnVision OS Netlify Deployment

Primary production domain:

- `https://pawnvision-os.com`

Planned domain structure:

- `https://pawnvision-os.com` = public site
- `https://www.pawnvision-os.com` = redirects to primary public site
- `https://app.pawnvision-os.com` = future broker app / dashboard host

## Netlify publish settings

This project is a static site.

- Publish directory: `.`
- Build command: none

## Required DNS records at IONOS

Keep mail-related records in place.

Website records:

- `A` record
  - Host: `@`
  - Value: `75.2.60.5`

- `CNAME` record
  - Host: `www`
  - Value: `[your-netlify-site].netlify.app`

Future app record:

- `CNAME` record
  - Host: `app`
  - Value: `[future-app-target]`

## Netlify domain setup

Attach:

- `pawnvision-os.com`
- `www.pawnvision-os.com`

Netlify should provision HTTPS/SSL after the DNS is pointed correctly.

## Notes

- Do not reconnect B12.
- Do not use any old temporary domain.
- Public pages explain and sell the product.
- The dashboard remains the internal broker operating system experience.
