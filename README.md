# Natours Project

This is a **Natours** project built for learning purposes using **HTML** and **SCSS**. The project was developed by following the **7-1 architecture pattern** in **Sass** and incorporates various features such as mixins, variables, custom animations, and more.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Folder Structure](#folder-structure)
- [Scripts](#scripts)
- [Custom Animations](#custom-animations)
- [SCSS Features](#scss-features)

## Features
- **7-1 Sass Architecture** pattern to organize SCSS files:
  - `base/` for global styles like typography.
  - `components/` for reusable components like buttons.
  - `layout/` for the main layout elements (header, footer, etc.).
  - `pages/` for page-specific styles.
  - `themes/` for color themes and variables.
  - `abstracts/` for functions, mixins, and variables.
  - `vendors/` for third-party stylesheets.
- **Custom Mixins** for repetitive styles.
- **Variables** to manage color schemes and font sizes.
- **Animations**: Custom animations are created using `@keyframes` in SCSS.
- Use of **BEM (Block Element Modifier)** methodology for naming classes in a clean and structured way.

## Technologies Used
- **HTML5**
- **SCSS (Sass)** with the **7-1 Architecture**

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/natours.git
   ```

2. Navigate to the project directory:
   ```bash
   cd natours
   ```

3. Install the dependencies:
   ```bash
   npm install
   ```

## Folder Structure
```plaintext
natours/
├── scss/
│   ├── abstracts/        # Variables, mixins, functions
│   ├── base/             # Base styles (e.g. typography, resets)
│   ├── components/       # Reusable UI components (e.g. buttons)
│   ├── layout/           # Global layout (e.g. header, footer)
│   ├── pages/            # Page-specific styles
│   ├── themes/           # Theme files (e.g. color schemes)
│   └── vendors/          # Third-party stylesheets
├── css/
│   └── main.css          # Compiled CSS file
├── js/
│   └── script.js         # JavaScript file
├── index.html            # Main HTML file
└── package.json          # Project dependencies and scripts
```

## Scripts

In your `package.json` file, you will find the following scripts:

### 1. Compile SCSS to CSS

This script compiles all your SCSS files into a single `main.css` file:

```bash
npm run compile:sass
```

To compile your SCSS files, just run the command above, and your SCSS will be converted to a single CSS file saved in the `css/` folder.

You can configure this script in your `package.json` like this:

```json
"scripts": {
  "compile:sass": "node-sass --watch scss/main.scss css/main.css"
}
```

This command also uses `--watch` to automatically recompile the SCSS whenever you make changes.

### 2. Live Server

For live reloading and preview of your project:

```bash
npm run start
```

This script runs a live server that serves your project and automatically reloads it upon changes to HTML, SCSS, or JavaScript files.

## Custom Animations

Animations are implemented using custom **SCSS `@keyframes`**. Some of the animations include:

- **Button Hover Animation**: Adds a smooth color transition effect when hovering over buttons.
- **Card Pop-In Animation**: A pop-in animation effect for displaying cards on the homepage.

