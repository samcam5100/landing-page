# Defiant Health GLP-1 Site

A static marketing and screening site for the GLP-1 weight management program. Plain HTML, no build step.

## Files

- index.html (home page, must keep this exact name so it serves as the front page)
- how-it-works.html, treatments.html, the-science.html, faq.html (core pages)
- learn.html (education hub) and the four learn articles
- privacy.html, terms.html, telehealth-consent.html, hipaa-notice.html (legal, placeholder text)
- defiant-science-molecule.svg (bonus graphic asset, reusable)
- Defiant_Health_GLP1_Guide.html (the lead magnet guide, not linked in the nav, host or export to PDF when ready)

All internal links use relative file names, so the site works as-is when deployed.

## Deploy with GitHub and Vercel

1. Create a new GitHub repository and upload every file in this folder to the root of the repo.
2. In Vercel, click Add New Project and import that repository.
3. When asked for a framework preset, choose Other. Leave the Build Command empty and leave the Output Directory as the root. There is no build step.
4. Click Deploy. Vercel gives you a live URL in under a minute.
5. After it looks good, add your custom domain under the project Settings, then Domains, and follow the DNS steps Vercel shows.

Every time you push a change to the repo, Vercel redeploys automatically.

## Before you point your real domain at it (pre-launch checklist)

The site is fully built but a few items are placeholders. Fill these in the CONFIG block near the bottom of each page (or ask for help wiring them):

Functional wiring (in the CONFIG block):
- questionnaireUrl: set to your real HIPAA-compliant intake form link. Until then the questionnaire is a demo and does not transmit anything.
- bookingUrl: set to your Calendly or Acuity link so the Book a consult buttons work.
- tracking.customEndpoint: set to your secure, BAA-covered endpoint for the email capture and any submissions. Keep health answers out of marketing tools.

Content placeholders to replace:
- Program price, currently shows [price]
- Provider titles and bios for Dr. Crane and Dr. Matt Leavitt
- Real consented patient quotes and the featured story
- Your Google profile link and clinic hours
- Real attorney-reviewed copy on the four legal pages

Compliance note: the questionnaire collects health information, so the tool that stores it needs a signed BAA, and the legal pages should be reviewed by your attorney before launch. This is a flag to confirm with your lawyer, not legal advice.
