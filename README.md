<div align="center">

# 🚀 Prime Fix's Landing Page 

[![Astro](https://img.shields.io/badge/Astro-5.13.6-FF5D01?style=for-the-badge&logo=astro&logoColor=white)](https://astro.build)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-4.1.13-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![Vercel](https://img.shields.io/badge/Vercel-Deploy-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com)
[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)

**A modern, multilingual landing page built with Astro and TailwindCSS**

[Demo](#) · [Report Bug](#) · [Request Feature](#)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Development](#development)
- [Available Scripts](#-available-scripts)
- [Internationalization](#-internationalization)
- [Deployment](#-deployment)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 🎯 Overview

This is a modern, responsive landing page built with **Astro** and styled with **TailwindCSS**. The project features a multi-language system, theme switching capabilities, and is optimized for deployment on Vercel.

## ✨ Features

- 🌐 **Multilingual Support** - Built-in internationalization (i18n) system
- 🎨 **Theme Switching** - Dark/Light mode toggle
- ⚡ **Lightning Fast** - Built with Astro for optimal performance
- 📱 **Fully Responsive** - Mobile-first design approach
- 🎯 **SEO Optimized** - Meta tags and semantic HTML
- 🚀 **Vercel Ready** - Pre-configured for seamless deployment
- 💅 **Modern Styling** - TailwindCSS v4 with Vite plugin
- 🔧 **Type Safety** - TypeScript configuration included

## 🛠️ Tech Stack

| Technology | Purpose | Version |
|------------|---------|---------|
| **[Astro](https://astro.build)** | Web Framework | 5.13.6 |
| **[TailwindCSS](https://tailwindcss.com)** | CSS Framework | 4.1.13 |
| **[TypeScript](https://www.typescriptlang.org/)** | Type Safety | Latest |
| **[Vercel](https://vercel.com)** | Deployment Platform | - |
| **[pnpm](https://pnpm.io/)** | Package Manager | Latest |

## 📁 Project Structure

```
landing-page/
├── public/                  # Static assets
│   └── assets/
│       ├── fonts/          # Custom fonts
│       └── images/         # Images and graphics
├── src/
│   ├── components/         # Reusable Astro components
│   │   ├── ChangeTheme.astro
│   │   ├── Feature.astro
│   │   ├── Footer.astro
│   │   ├── Header.astro
│   │   ├── Home.astro
│   │   ├── HomeCard.astro
│   │   ├── HomeGuide.astro
│   │   ├── HomePresentation.astro
│   │   └── SelectLang.astro
│   ├── i18n/               # Internationalization
│   │   ├── ui.ts          # Translation strings
│   │   └── utils.ts       # i18n utilities
│   ├── layouts/            # Page layouts
│   │   ├── Layout.astro
│   │   └── LayoutWorking.astro
│   ├── pages/              # File-based routing
│   │   ├── index.astro
│   │   └── [lang]/        # Dynamic language routes
│   │       ├── features.astro
│   │       ├── index.astro
│   │       └── working.astro
│   └── styles/
│       └── global.css      # Global styles
├── astro.config.mjs        # Astro configuration
├── package.json            # Dependencies
├── tsconfig.json           # TypeScript configuration
└── README.md               # Documentation
```

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v18.0.0 or higher)
- **pnpm** (v8.0.0 or higher)

```powershell
# Check Node.js version
node --version

# Check pnpm version
pnpm --version

# Install pnpm if needed
npm install -g pnpm
```

### Installation

1. **Clone the repository**

```powershell
git clone https://github.com/prime-fix-app-web/landing-page.git
cd landing-page
```

2. **Install dependencies**

```powershell
pnpm install
```

### Development

Start the development server:

```powershell
pnpm dev
```

The application will be available at `http://localhost:4321`

## 📜 Available Scripts

| Command | Description |
|---------|-------------|
| `pnpm dev` | Starts the development server with hot reload |
| `pnpm build` | Builds the project for production |
| `pnpm preview` | Previews the production build locally |
| `pnpm astro` | Access Astro CLI commands |

## 🌐 Internationalization

The project includes a built-in internationalization system supporting multiple languages.

### Adding a New Language

1. Add translations in `src/i18n/ui.ts`
2. Create language-specific routes in `src/pages/[lang]/`
3. Update the language selector component

### Usage Example

```astro
---
import { getLangFromUrl, useTranslations } from '../i18n/utils';

const lang = getLangFromUrl(Astro.url);
const t = useTranslations(lang);
---

<h1>{t('welcome')}</h1>
```

## 🚢 Deployment

### Deploy to Vercel

This project is pre-configured for Vercel deployment:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/prime-fix-app-web/landing-page)

#### Manual Deployment

1. **Install Vercel CLI**

```powershell
pnpm add -g vercel
```

2. **Deploy**

```powershell
vercel
```

3. **Production Deployment**

```powershell
vercel --prod
```

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 📧 Contact

**Project Link:** [https://github.com/prime-fix-app-web/landing-page](https://github.com/prime-fix-app-web/landing-page)

---

<div align="center">

**Made using Astro and TailwindCSS**

</div>
