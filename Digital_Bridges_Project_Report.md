**PROJECT REPORT**

**Digital Bridges**

Inclusive Digital Literacy Training Content Development for Communities in Zambia

*Zambian Cyber Security Initiative Foundation (ZCSIF)*

*Prepared: June–July 2026 • Covers: Phase 2 – Curriculum and Content Design*

# **1. Executive Summary**

Digital Bridges is a new digital literacy training program developed by the Zambian Cyber Security Initiative Foundation (ZCSIF) to help close Zambia's digital divide. The program was established under the Foundation's concept note, “Digital Literacy Training Content Development,” which set out a goal of delivering accessible, practical, and locally relevant digital literacy training to underserved communities across Zambia, along with a four-phase implementation strategy for getting there.

This report documents the work completed under Phase 2 of that strategy: Curriculum and Content Design. It covers the design and development of the eight training modules identified in the concept note, and the digital platform built to deliver them — a 10-page website comprising a Home page, an About page, and the eight training modules, supported by a navigation, branding, and contact system aligned with the Foundation's identity.

The platform is a lightweight, dependency-free build — plain HTML, CSS, and vanilla JavaScript across all 10 pages — and was validated throughout development with automated HTML parsing, link-integrity checks, and headless-browser testing of its interactive features.

# **2. Program Background**

Digital technologies increasingly shape access to education, employment, entrepreneurship, public services, and civic life. Many young people, women, informal workers, rural communities, and other marginalized groups in Zambia continue to face real barriers to accessing and effectively using digital tools, and existing digital literacy materials are often too technical, not localized, or disconnected from the everyday realities communities face.

Digital Bridges was conceived to close that gap with training content that is practical, inclusive, and adaptable — covering online safety, misinformation, digital financial services, responsible social media use, productivity tools, and digital entrepreneurship — delivered through a platform that communities can access directly.

# **3. Program Goal & Objectives**

Goal: to develop accessible, practical, and locally relevant digital literacy training content that strengthens digital skills, online safety awareness, and meaningful digital participation among underserved communities in Zambia.

* Design a comprehensive digital literacy curriculum tailored for youth, women, community groups, and informal sector workers.
* Develop easy-to-understand training materials suitable for both online and offline learning environments.
* Integrate digital safety, cyber hygiene, misinformation awareness, and responsible technology use into every training module.
* Create interactive, community-friendly learning tools that improve engagement and retention.
* Support trainers, educators, and community facilitators with adaptable teaching resources.

# **4. Implementation Strategy**

The concept note sets out a four-phase implementation strategy for the program. This report documents Phase 2; the table below shows how it fits into the full roadmap.

| **Phase** | **Focus** | **Key Activities** | **Status** |
| --- | --- | --- | --- |
| Phase 1 | Needs Assessment | Stakeholder consultations; community digital literacy mapping; identification of priority learning gaps. | Precedes this report |
| Phase 2 | Curriculum and Content Design | Development of the learning framework; module writing and visual design; build-out of the training platform. | Completed — this report |
| Phase 3 | Pilot Testing | Community testing sessions; trainer feedback collection; content refinement. | Planned next |
| Phase 4 | Deployment and Capacity Building | Distribution of training materials; training-of-trainers sessions; community learning workshops. | Enabled by the platform; rollout planned |

# **5. Phase 2 Deliverables: Curriculum & Platform**

The following deliverables were completed under Phase 2 — Curriculum and Content Design:

| **Deliverable** | **Description** |
| --- | --- |
| Learning framework & platform architecture | A 10-page digital platform structured around a Home page, an About page, and the eight proposed training content areas from the concept note. |
| Module writing & visual design | Each of the eight training content areas was written up as a full module — objective, learning outcomes, core content, and reflection or self-check activities — and given a consistent visual design. |
| Navigation & wayfinding system | A horizontal, sticky navigation bar with a condensed “Training” dropdown for larger screens, and a hamburger-triggered slide-out menu with a matching Training accordion for smaller screens. |
| Program identity pages | A Home page introducing the program and a dedicated About page describing the Foundation's mission and the program's purpose, both aligned with ZCSIF's brand and public identity. |
| Contact & outreach footer | A footer carrying the Foundation's address, phone, email, and social channels, designed to expand into full view as a visitor reaches the bottom of a page. |

# **6. Platform Structure**

The delivered platform consists of ten pages, all sharing a common header, navigation, and footer:

| **Page** | **File** | **Purpose** |
| --- | --- | --- |
| Home | index.html | Program introduction, value proposition, curriculum overview, and a link back to the Foundation's main site. |
| About | about.html | Foundation mission, program background, values, and contact information. |
| Intro to Digital Literacy | intro.html | Digital devices, smartphone and computer basics, and internet navigation. |
| Online Safety & Cyber Hygiene | safety.html | Password management, scam and phishing awareness, and safe online behavior. |
| Digital Communication | communication.html | Email etiquette, messaging platforms, video conferencing, and digital teamwork. |
| Information & Media Literacy | inform.html | Identifying misinformation, fact-checking, and responsible content sharing. |
| Digital Financial Literacy | financial.html | Mobile money safety, digital payments, and fraud awareness. |
| Productivity & Work Readiness | productivity.html | Document creation, internet research, and CV/digital profile development. |
| Digital Entrepreneurship | entrepreneurship.html | Social media marketing, online customer engagement, and e-commerce basics. |
| Responsible Digital Citizenship | citizenship.html | Ethical technology use, digital rights, and wellbeing in digital spaces. |

# **7. Platform Features**

## **7.1 Navigation**

* Desktop (larger screens): a horizontal, sticky nav bar sits under the site header at all times, containing Home, About, and a Training dropdown.
* The Training dropdown condenses the eight module links into a single menu, opened on hover or click, closing automatically when a selection is made or the user clicks elsewhere.
* Mobile (smaller screens): the horizontal bar is replaced by a hamburger icon that opens a slide-out sidebar; the eight module links are grouped under a tappable Training accordion to keep the menu short.
* The active page is highlighted in both the top-level nav and, where applicable, within the Training dropdown/accordion.

## **7.2 Home & About Pages**

* Home: hero banner introducing the program, a “why this training” value grid, the full eight-module curriculum grid, and a call-to-action linking to zcsi-foundation.org.
* About: Foundation mission and background, the Digital Bridges program story, an approach/values grid, and a dedicated contact block.
* Content and contact details (address, phone, email, and social handles) were sourced from ZCSIF's public web presence to keep the platform consistent with the Foundation's identity.

## **7.3 Footer**

* Default state: a plain, single-line sticky bar showing only the copyright notice.
* Expanded state: scrolling any page to the bottom reveals the full footer — street address, phone, email, and social links — mirroring the reveal-on-scroll footer pattern used on the Foundation's main site.
* Street address: Woodlands Mosi Tunya Road, Corner of Nalikwanda Road Plot 2, Lusaka, Zambia.

## **7.4 Development Quality Checks**

The following issues were identified and resolved during development, before the platform was finalized:

* Corrected mismatched HTML tag nesting in an early version of the header/sidebar markup that prevented the intended sidebar layout from rendering.
* Corrected a CSS media query that was closing early, which had left mobile-only hamburger/sidebar rules applying at all screen widths.
* Corrected an incorrect “active” navigation highlight on the Online Safety module.
* Removed a duplicated footer element and leftover unused JavaScript from an earlier iteration of the Financial Literacy module.

# **8. Technical Notes**

**Stack:** static HTML5, CSS3 (custom properties, flexbox), and vanilla JavaScript — no build step, framework, or external runtime dependency beyond a Google Fonts stylesheet for the Material Symbols home icon.

**Layout model:** each page scrolls within an inner content panel rather than the full document, which keeps the header and navigation permanently in view without relying on fixed positioning.

**Shared components:** navigation, footer, and the responsive/menu JavaScript are duplicated consistently across all 10 static pages (there is no shared templating layer), so future content edits to the header, nav, or footer need to be applied to each file.

**Dependencies:** none requiring installation; the Google Fonts stylesheet link is the only external asset.

# **9. Testing & Quality Assurance**

* HTML validity: every page parsed with a browser-equivalent HTML5 parser after each change to confirm no malformed markup.
* Link integrity: all internal hrefs were checked programmatically to confirm they resolve to existing pages.
* Headless-browser verification (Chromium via Playwright) at desktop, tablet, and mobile breakpoints, checking:
  + Correct show/hide of the horizontal nav bar vs. the hamburger/sidebar at the 768px breakpoint
  + Dropdown and accordion open/close behavior on hover, click, and navigation
  + Footer collapse/expand behavior when scrolling to the bottom of the page
  + Absence of JavaScript console errors on every page
* Visual review of rendered screenshots to confirm layout, spacing, and branding matched intent.

# **10. Sustainability & Partnerships**

In line with the concept note, the platform is intended as an open, adaptable resource that schools, civil society organizations, youth hubs, and community centers can reuse and build on. Longer-term reach depends on partnerships the Foundation is positioned to pursue with schools and universities, community radio stations, youth and civil society organizations, ICT hubs, government ICT and education institutions, and telecommunications companies.

# **11. Recommendations & Next Steps**

* Confirm that the eight training content areas built in Phase 2 reflect any findings from Phase 1 (Needs Assessment) consultations and community mapping, and adjust module emphasis if gaps are identified.
* Proceed to Phase 3 (Pilot Testing): run community testing sessions on the live platform, collect trainer feedback, and refine content based on results.
* Plan Phase 4 (Deployment and Capacity Building): training-of-trainers sessions and community learning workshops to actively distribute and teach from the platform, beyond simply publishing it.
* The concept note calls for multilingual, locally adapted content; the current platform is English-only, so translation and localization remains outstanding work ahead of full deployment.
* Consider a lightweight build step (e.g., a static-site generator or simple templating) if the header, nav, or footer will need frequent updates — this would remove the need to edit all 10 files by hand for shared changes.