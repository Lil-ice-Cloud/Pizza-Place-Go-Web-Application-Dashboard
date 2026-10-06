# Pizza Place Dashboard

A modern, responsive analytics dashboard for Pizza Place, built with Next.js and
Shadcn UI. The project provides a clean workspace for monitoring business
metrics, reviewing activity, managing projects, and collaborating with a team.

## Highlights

- **Shadcn UI dashboard experience** with accessible, reusable components for
  cards, buttons, navigation, dialogs, forms, tables, tabs, tooltips, and more.
- **Responsive application shell** with a collapsible sidebar, header,
  breadcrumbs, navigation groups, documents, settings, search, and user menu.
- **Dashboard overview** with summary metric cards, an interactive chart area,
  and a sortable data table for activity and performance data.
- **Team-ready navigation** with dedicated Dashboard, Lifecycle, Analytics,
  Projects, and Team sections, plus a user profile area.
- **Light and dark mode** powered by `next-themes`, including system theme
  detection and theme-aware Shadcn color tokens.
- **Local Poppins typography** with multiple weights and italic variants for a
  consistent visual identity.
- **Responsive layouts** designed for desktop, tablet, and mobile screen sizes.

## Tech stack

- [Next.js](https://nextjs.org/) 16 with the App Router
- [React](https://react.dev/) 19
- [TypeScript](https://www.typescriptlang.org/)
- [Shadcn UI](https://ui.shadcn.com/) and Tailwind CSS
- [Lucide React](https://lucide.dev/) icons
- [Recharts](https://recharts.org/) for data visualization
- [TanStack Table](https://tanstack.com/table) for dashboard tables
- [next-themes](https://github.com/pacocoursey/next-themes) for light/dark mode

## Getting started

### Prerequisites

- Node.js 20 or later
- npm, pnpm, yarn, or Bun

### Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/Lil-ice-Cloud/Pizza-Place-Go-Web-Application-Dashboard.git
cd Pizza-Place-Go-Web-Application-Dashboard
npm install
```

### Run the development server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Available scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Next.js development server |
| `npm run build` | Create a production build |
| `npm run start` | Serve the production build |
| `npm run lint` | Run ESLint |

## Project structure

```text
app/
├── dashboard/
│   ├── data.json          # Dashboard table data
│   └── page.tsx           # Dashboard layout and sections
├── globals.css            # Theme tokens and global styles
├── layout.tsx             # Root layout, fonts, and theme provider
└── page.tsx               # Application entry point

components/
├── ui/                    # Shadcn UI building blocks
├── app-sidebar.tsx        # Main dashboard navigation
├── chart-area-interactive.tsx
├── data-table.tsx
├── section-cards.tsx
└── site-header.tsx
```

## Theming

The dashboard uses `next-themes` with class-based theme switching. It starts
with the user's system preference and supports light and dark color tokens
defined in `app/globals.css`. Components use the same semantic tokens in both
themes, so cards, charts, tables, borders, and sidebar navigation remain
consistent when the theme changes.

## Customization

- Update dashboard navigation and team sections in
  `components/app-sidebar.tsx`.
- Replace sample dashboard records in `app/dashboard/data.json`.
- Adjust summary cards, charts, and table behavior in the corresponding files
  under `components/`.
- Customize colors, spacing, radii, and dark mode values in
  `app/globals.css`.
- Add or extend Shadcn UI primitives in `components/ui/` as the dashboard
  grows.

## Deployment

The application can be deployed to any platform that supports Next.js. For the
quickest deployment, import the repository into
[Vercel](https://vercel.com/new) and configure the project using the standard
Next.js build settings.

Before deploying, verify the production build locally:

```bash
npm run lint
npm run build
```

## License

This project is maintained as a Pizza Place dashboard application. Add the
appropriate license here if the project is distributed publicly.
