<div align="center">

# Hermanos Mendoza

### Website for a custom carpentry and painting workshop

A modern, responsive landing page designed to present the services, projects, and contact channels of **Carpintería y Pintura Hermanos Mendoza**.

</div>

---

## About the project

This project turns the digital presence of a local workshop into a clear and trustworthy experience for potential customers. The website explains the work process, presents finished projects, answers common questions, and makes it easy to request a quote.

The interface was designed to help users:

- Quickly understand the workshop's services.
- Explore previous work and learn about its value.
- Find answers to common questions without leaving the page.
- Request a quote through WhatsApp or make a phone call.

## Key features

- Responsive design for mobile, tablet, and desktop.
- Mobile navigation with an accessible menu that can be closed with `Escape`.
- Dedicated sections for services, projects, frequently asked questions, and contact.
- Clear calls to action focused on quote requests.
- Content separated from the presentation layer through JSON files.
- Reusable Astro components for buttons, the header, and the footer.
- A consistent visual system and typography using Tailwind CSS.
- External links configured with secure practices (`noopener noreferrer`).

## Tech stack

| Technology                               | Purpose                                      |
| ---------------------------------------- | -------------------------------------------- |
| [Astro](https://astro.build/)            | Main framework and interface generation      |
| [Tailwind CSS](https://tailwindcss.com/) | Responsive styles and utility classes        |
| TypeScript                               | Type safety and strict project configuration |
| JSON                                     | Project, benefits, and FAQ content           |
| Vercel                                   | Demo deployment                              |

## Project structure

```text
.
├── public/                 # Favicon and public files
├── src/
│   ├── assets/             # Logo and visual assets
│   ├── components/
│   │   ├── ui/             # Reusable buttons
│   │   ├── Footer.astro
│   │   ├── Header.astro
│   │   └── Main.astro
│   ├── data/               # Editable page content
│   │   ├── cards.json
│   │   ├── faqs.json
│   │   └── projects.json
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## Run the project locally

### Requirements

- Node.js `22.12.0` or higher.
- npm.

### Installation

```bash
git clone https://github.com/marioswc/hermanos-mendoza.git
cd hermanos-mendoza
npm install
```

### Development

```bash
npm run dev
```

The application will be available at [http://localhost:4321](http://localhost:4321).

### Other commands

| Command                   | Description                                                        |
| ------------------------- | ------------------------------------------------------------------ |
| `npm run build`           | Generates the optimized version in `dist/`.                        |
| `npm run preview`         | Serves the generated version locally for review before deployment. |
| `npm run astro -- --help` | Displays the Astro CLI help.                                       |

## Live demo

Visit the published version at [hermanos-mendoza.vercel.app](https://hermanos-mendoza.vercel.app/).
