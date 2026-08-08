# Agent Browser

<!-- prettier-ignore-start -->
<div align="center">

![Next.js](https://img.shields.io/badge/Next.js-16-black?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![Bun](https://img.shields.io/badge/Bun-Servlet-000000?style=for-the-badge&logo=bun&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**A modern, fast, and extensible web browser interface built with Next.js 16.**

[Features](#features) · [Quick-start](#quick-start) · [Tech-stack](#tech-stack) · [Contributing](CONTRIBUTING.md) · [License](LICENSE)

</div>
<!-- prettier-ignore-end -->

## Features

- **Next.js 16** — The latest version of the React framework with Turbopack for lightning-fast development
- **React 19** — With all the newest patterns and features
- **TypeScript 5** — Full type safety across the codebase
- **Tailwind CSS v4** — Utility-first styling with the latest engine
- **shadcn/ui Components** — Beautifully designed, accessible, copy-and-paste components (base-nova style)
- **Dark Mode** — Built-in theme switching with next-themes
- **Geist Font** — Clean, modern typography with sans and mono variants
- **Radix UI Primitives** — Accessible, unstyled component primitives under the hood
- **Bun** — Blazing-fast JavaScript runtime and package manager

## Quick Start

### Prerequisites

- [Bun](https://bun.sh/) >= 1.0 (or Node.js >= 20)

### Installation

```bash
# Clone the repository
git clone https://github.com/Lostovayne/Agent-browser.git
cd Agent-browser

# Install dependencies
bun install

# Start the development server
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

### Available Scripts

| Command        | Description                    |
| -------------- | ------------------------------ |
| `bun dev`      | Start development server       |
| `bun build`    | Build for production           |
| `bun start`    | Start production server        |
| `bun lint`     | Run ESLint                     |
| `bun typecheck`| Run TypeScript type checking   |
| `bun format`   | Format code with Prettier      |

## Project Structure

```
Agent-browser/
├── app/                  # Next.js App Router
│   ├── globals.css       # Global styles with Tailwind
│   ├── layout.tsx        # Root layout
│   └── page.tsx          # Home page
├── components/
│   ├── theme-provider.tsx
│   └── ui/               # shadcn/ui components (50+ components)
├── hooks/                # React hooks
├── lib/                  # Utility functions
├── public/               # Static assets
├── .prettierrc           # Prettier configuration
├── components.json       # shadcn/ui configuration
├── eslint.config.mjs     # ESLint configuration
├── next.config.ts        # Next.js configuration
├── postcss.config.mjs    # PostCSS configuration
├── tsconfig.json         # TypeScript configuration
└── package.json
```

## Adding Components

To add more shadcn/ui components to your app:

```bash
bunx shadcn@latest add button
```

This places UI components in `components/ui/`.

### Using Components

```tsx
import { Button } from "@/components/ui/button"
```

## Tech Stack

| Category        | Technology                          |
| --------------- | ----------------------------------- |
| Framework       | Next.js 16 (App Router)             |
| UI Library      | React 19                            |
| Language        | TypeScript 5                        |
| Styling         | Tailwind CSS v4                     |
| UI Components   | shadcn/ui + Radix UI                |
| Icons           | Lucide React                        |
| Theme           | next-themes                         |
| Package Manager | Bun                                 |
| Linter          | ESLint 9 (eslint-config-next)       |
| Formatter       | Prettier + prettier-plugin-tailwind |

## Contributing

We welcome contributions! Please see our [Contributing Guide](CONTRIBUTING.md) for details on how to get started, our code of conduct, and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [shadcn/ui](https://ui.shadcn.com/) for the incredible component system
- [Vercel](https://vercel.com/) for Next.js
- [Radix UI](https://www.radix-ui.com/) for accessible primitives
- [Tailwind Labs](https://tailwindcss.com/) for Tailwind CSS
