<div align="center">

# Maestro Sports website

**A production website I designed, built and deployed for an international football management company in Dubai and Ghana.**

[Live site](https://maestrosportsmanagement.com) · [Demo video](https://github.com/7kbytes/maestrosports-showcase/releases/download/v1.0/maestro-demo.mp4) · [How it works](#how-it-works) · [Contact](#contact)

![Maestro Sports walkthrough](assets/walkthrough.gif)

</div>

> This is a portfolio showcase of my work. The source code is private, and nothing here is open for reuse. See [All Rights Reserved](#all-rights-reserved).

## The brief

Maestro Sports scouts football talent in Ghana and West Africa and places it with clubs in the UAE and the Middle East. They needed a site that looks credible to clubs, sponsors and government partners, shows their real match photography, works well on phones, and turns visitors into enquiries.

## What I built

A five-page marketing site (Home, Services, About, News, Contact) with a privacy page, built with Next.js and deployed to Vercel. Visitors send enquiries through a form that emails the Maestro team directly, with replies going straight back to the visitor.

## Engineering highlights

- **Page weight.** The site uses full-resolution match photography. I found the hero alone was shipping 4.9 MB, so I turned image optimisation back on and shrank the source images. Photos are now resized and re-encoded per device.
- **A dependable contact pipeline.** Enquiries are validated on the server and sent by email from the company's own verified domain. The endpoint reports missing configuration and rejected emails clearly, rather than crashing or telling a visitor their message was sent when it was not.
- **Mobile first.** I fixed headline clipping, text overflow and a long email address wrapping mid-word, each checked at phone width on the live site.
- **Motion with restraint.** Animated hero, scroll reveals and gallery transitions with Framer Motion and GSAP.
- **Lean dependencies.** I removed unused design-exploration components and their libraries, so the production build ships only what the pages use.
- **Search ready.** Page metadata, Open Graph tags, a sitemap and robots rules.

## Screenshots

| Home | Services |
| --- | --- |
| ![Home](assets/shots/desktop-home.png) | ![Services](assets/shots/desktop-services.png) |

| About | Contact |
| --- | --- |
| ![About](assets/shots/desktop-about.png) | ![Contact](assets/shots/desktop-contact.png) |

| Mobile home | Mobile services | Mobile about | Mobile contact |
| --- | --- | --- | --- |
| <img src="assets/shots/mobile-home.png" width="180" alt="Mobile home"> | <img src="assets/shots/mobile-services.png" width="180" alt="Mobile services"> | <img src="assets/shots/mobile-about.png" width="180" alt="Mobile about"> | <img src="assets/shots/mobile-contact.png" width="180" alt="Mobile contact"> |

Captured from the live website, on desktop and at phone width.

## How it works

![Maestro Sports system architecture](assets/architecture.svg)

## Tech stack

| Area | Technology |
| --- | --- |
| Framework | Next.js 15 (App Router), React 19, TypeScript |
| Styling | Tailwind CSS 4, Google Fonts via next/font |
| Motion | Framer Motion, GSAP |
| Images | Next.js image optimisation, Cloudinary |
| Email | Resend, from a verified company domain |
| Hosting | Vercel, deployed from GitHub |

## My role

I handled design, front-end development, the contact backend, email setup, deployment and ongoing fixes, working directly with the client.

## Contact

- **GitHub:** [@7kbytes](https://github.com/7kbytes)

## All Rights Reserved

© 2026 7Kbytes. All Rights Reserved. Nothing in this repository may be copied, modified, distributed or reused without prior written permission. The Maestro Sports name, logo and photography belong to their owners and are shown with permission. See [LICENSE](LICENSE).
