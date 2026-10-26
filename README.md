# Aldrich A. Alimpolos — Personal CV Website

A responsive personal curriculum vitae and portfolio for IT415, presenting Aldrich's profile, career objective, education, skills, academic project, and contact information.

## Student

- **Name:** Aldrich A. Alimpolos
- **Program:** Bachelor of Science in Information Technology
- **School:** Davao del Norte State College
- **Year / Section:** 4th Year / BSIT 4D
- **Major:** Software Development
- **Subject:** IT415

## Technologies

HTML5, CSS3, and vanilla JavaScript. No dependencies or build step.

## Features

- Responsive desktop, tablet, and mobile layouts
- Mobile navigation, active section indicators, and smooth anchor scrolling
- Scroll reveals, hover interactions, and reduced-motion support
- Keyboard focus styles, skip navigation, semantic sections, and accessible menu state
- Print / save CV button with a dedicated print stylesheet (choose Save as PDF in the print dialog)
- Email, telephone, GitHub, and LinkedIn links
- TESDA Computer Systems Servicing NC II qualification and validity dates
- Cisco Networking Academy course completion certificate with local preview and PDF link
- Local assets and typography with no third-party runtime requests

## Files

```text
index.html     Content and semantic page structure
styles.css     Layout, responsive styles, animation, and print styles
script.js      Menu, section indicators, reveals, and print action
vercel.json    Static deployment configuration
README.md      Project documentation and deployment instructions
assets/certificates/  Cisco certificate PDF and preview image
assets/aldrich-profile.jpg  Profile photograph
```

## Preview locally

Open `index.html` directly, or run the following from this folder:

```sh
python -m http.server 3000
```

Then visit http://localhost:3000. No installation is needed.

## Repository and live website

- **GitHub repository:** https://github.com/ALdrich06/aldrich-cv-portfolio
- **Live Vercel URL:** https://aldrich-cv-portfolio.vercel.app

## Deploy to Vercel

1. Review changes with `git diff`, then commit and push this folder to the dedicated repository above. Preserve existing history and use meaningful commits for subsequent changes.
2. In Vercel, choose **Add New → Project** and import `ALdrich06/aldrich-cv-portfolio`.
3. Select the repository root as the Root Directory and **Other** as the Framework Preset. No build command is required. Serve the repository root (`.`) as the output directory.
4. Deploy, open the generated production URL, and verify desktop and mobile layouts, navigation, print output, contact links, and GitHub links.
5. Replace the pending live URL in this README with the verified Vercel URL, commit, and push.
6. Submit the public Vercel URL and GitHub repository URL to the LMS.

## Content still needed before final submission

- Profile photo is included at `assets/aldrich-profile.jpg`, using the supplied image with responsive sizing and descriptive alt text.
- Add verified projects and their descriptions, technologies, screenshots, and repository/live links when available. The current project is this actual CV website.
- Cisco course completion certificate is included: CCNA: Switching, Routing, and Wireless Essentials, completed December 1, 2025.
- TESDA Computer Systems Servicing NC II is included: issued December 27, 2023, valid until December 26, 2028. The original PDF was reviewed locally; its password, certificate number, ULI, and full document are not included in the public source.
- Add further verified achievements, seminars, or relevant experience if applicable.
- LinkedIn is linked at https://www.linkedin.com/in/aldrich-alimpolos-69450042a/. Add other public profiles only when their real URLs are available.
- Confirm that the existing education dates, year level, contact details, and public phone number are current and intended for publication.

No work history, credentials, account links, or project accomplishments have been invented. The Cisco entry describes course completion, rather than claiming the separate CCNA professional certification exam.

## Manual verification

Check at 375px (phone), 768px (tablet), and 1440px (desktop): readable text, no horizontal overflow, usable navigation, visible focus states, and correct project layout. Test the mobile Menu button and Escape key, each navigation anchor, email/phone/GitHub links, reduced-motion mode, JavaScript-disabled navigation, and Print / save CV.

## Collaborative academic projects

The student confirmed Aldrich served as a developer for CoopNexus (capstone, in development), BananaGuard (Data Mining), and PlayMate (HCI and Technopreneurship). Project descriptions and technology context come from the shared academic portfolio at https://github.com/pearlsulana/pearlsulana.github.io. Links lead to teammate Pearl's project previews; no unverified source-code repository links are claimed.

## Project detail pages

`capstone.html`, `data-mining.html`, and `hci-techno.html` provide local project details with selected original project visuals and a responsive layout. The design is specific to this CV. PlayMate live demo: https://playmate-chess.netlify.app/. Source project visuals are retained from the shared academic portfolio.
