# Apps

A clean, modern portfolio page showcasing my personal projects and applications. Built with Astro for maximum performance and simplicity.

## Features

- Static site generation (no client-side JavaScript)
- Responsive design with mobile-first approach
- Light and dark mode support via `prefers-color-scheme`
- CSS Grid with subgrid for consistent alignment
- Accessible, semantic HTML
- Clean, professional aesthetic

## Tech Stack

- **Astro** - Static site generator
- **TypeScript** - Type safety
- **CSS** - Modern CSS with Grid, custom properties, and media queries
- **Inter** - Clean, professional typeface from Google Fonts

## Project Structure

```
/
├── public/
│   ├── icons/          # App icons (SVG/PNG)
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── AppTile.astro   # Reusable app tile component
│   └── pages/
│       └── index.astro     # Main landing page
└── package.json
```

## Development

### Prerequisites

- Node.js 18 or higher
- npm

### Getting Started

1. Install dependencies:

   ```sh
   npm install
   ```

2. Start the development server:

   ```sh
   npm run dev
   ```

3. Open your browser to `http://localhost:4321`

### Building for Production

```sh
npm run build
```

The static site will be generated in the `./dist/` directory.

### Preview Production Build

```sh
npm run preview
```

## Adding New Apps

To add a new app to the listing, edit `src/pages/index.astro` and add a new `<AppTile>` component with the following props:

```astro
<AppTile
  name="App Name"
  subtitle="Brief description of what the app does"
  icon="app-icon.svg"
  productionUrl="https://example.com"
  githubUrl="https://github.com/username/repo"
/>
```

Place the corresponding icon file in the `public/icons/` directory.

## License

Private project for personal use.
