# web-drawing-svg

A lightweight web-based drawing application that uses SVG for vector drawing in the browser. Build freehand and basic-shape drawings, edit strokes, and export as SVG or PNG. Designed to be simple, extensible, and easy to integrate into other web projects.

## Features

- Freehand drawing with smooth SVG paths
- Basic shapes: rectangle, circle, line
- Color and stroke-width selection
- Undo / redo
- Clear canvas
- Export as SVG or PNG
- Keyboard shortcuts for common actions
- Small and dependency-light (works in modern browsers)

## Demo

Open `index.html` in a browser or run the dev server to see the app in action. (If the repository includes a demo link, replace this with the hosted URL.)

## Quick Start

Prerequisites:
- Node.js (16+) and npm (if using the development server / build pipeline)
- A modern web browser

Clone the repo and run locally:

```bash
git clone https://github.com/Winstonjames2/web-drawing-svg.git
cd web-drawing-svg
npm install
npm run dev   # or `npm start` depending on the project scripts
```

If the project is plain static HTML/CSS/JS, you can just open `index.html` in your browser.

## Usage

- Select a tool from the toolbar (Pen, Rectangle, Circle, Line, Select/Eraser).
- Pick color and stroke width from the controls.
- Draw on the canvas area. Use Undo / Redo buttons to revert changes.
- Export:
  - Export SVG to keep vector quality.
  - Export PNG to get a rasterized image (useful for sharing).

Example: Export SVG by clicking "Export" > "Download SVG".

## Development

Project layout (example — adjust to match the repo):

- `index.html` — main entry / demo page
- `src/` — application JS and CSS source files
- `public/` — static assets (icons, fonts)
- `dist/` — built output (if you use a bundler)
- `README.md` — this file

Scripts (example):
- `npm run dev` — start dev server with live reload
- `npm run build` — build production bundle
- `npm test` — run tests

If you use a bundler like Vite/Parcel/webpack, ensure the dev script runs the bundler and serves the app.

## Extending and Integration

This app is designed to be embedded or extended:
- Expose the current SVG DOM for integration with other UI components.
- Provide hooks to save/load drawings from a server.
- Add shape snapping, alignment, grouping, and layers for more advanced editing.

## Contributing

Contributions are welcome! Suggested process:
1. Fork the repository.
2. Create a feature branch
3. Make your changes and add tests where applicable.
4. Open a pull request describing your changes.

Please follow standard commit message conventions and keep changes focused.

## Troubleshooting

- If strokes appear jagged: smooth your path generation or increase sampling frequency.
- If export size is large: simplify paths or remove unnecessary metadata before exporting.

## License

This project is available under the MIT License. See LICENSE file for details.

## Contact

For questions or help, open an issue on the repository or contact [kyawhtetmyattun@gmail.com]
