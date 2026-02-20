# StoryCast – Digital Storytelling Platform

StoryCast is a high-impact, accessible digital storytelling platform dedicated to conspiracy narratives through audio documentaries and articles.

## Project Structure

- `index.html`: The homepage featuring the hero section and trending stories carousel.
- `about.html`: An informational page detailing our mission and accessibility commitment.
- `story/`: Directory containing long-form story pages (e.g., `story1.html`).
- `sass/`: Modular SCSS files following the 7-1 pattern:
  - `abstracts/`: Variables, mixins, and base styles.
  - `layout/`: Header, footer, and grid systems.
  - `components/`: Reusable UI elements like cards, hero, and carousels.
- `css/`: Production-ready compiled CSS (`main.css`).
- `assets/`: Project assets including images, audio files, and WebVTT transcripts.

## Accessibility Checklist

StoryCast is built with a "Privacy and Accessibility First" mindset, meeting **WCAG 2.1 Level AA** standards:

- **Semantic HTML5**: Proper use of landmark elements (`<header>`, `<main>`, `<nav>`, `<footer>`) and sectioning (`<article>`, `<section>`).
- **Skip Navigation**: A skip-link is present on all pages to allow keyboard users to bypass repeated navigation.
- **Keyboard Operability**: All interactive elements (buttons, links, audio controls) are fully navigable via `Tab` and `Enter`.
- **Aria Labels**: Screen readers can accurately identify and describe UI components.
- **No-JS Fallback**: Implemented a for responsive navigation on subpages, ensuring mobile menus work without JavaScript.
- **Text Transcripts**: Audio documentaries include full timestamped transcripts.
- **Alt Text**: Meaningful descriptions for all functional images.

## Instructions for Running Locally

To run this project on your local machine, follow these steps:

### 1. View Pages
Simply open `index.html` in any modern web browser. No specialized server is required for basic viewing.

### 2. Sass Compilation (Development)
If you wish to modify the styles, you will need to recompile the Sass files:

1. Ensure you have [Node.js](https://nodejs.org/) installed.
2. Open your terminal in the project root.
3. Run the following command to compile Sass:
   ```bash
   npx sass sass/main.scss css/main.css
   ```
4. To watch for changes automatically:
   ```bash
   npx sass --watch sass/main.scss:css/main.css
   ```

### 3. Dependencies
This project prides itself on being lightweight and dependency-free. It uses standard HTML5, CSS3 (compiled from Sass), and minimal Vanilla JavaScript.
