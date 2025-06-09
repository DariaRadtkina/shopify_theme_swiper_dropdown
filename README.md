# Shopify Product Swiper Gallery with Color Filtering and Dynamic Dropdown
## Overview 🔧
This project showcases a flexible and responsive product gallery for Shopify stores. Built with Swiper.js, it allows merchants to control the gallery layout for different screen sizes and dynamically filter product images based on selected color variants. It also features a customizable dropdown, sourced directly from product metafields, making it easy to extend product pages without touching the code.

## Tech Stack 🛠
- Shopify Liquid;
- JavaScript;
- Swiper.js;
- HTML/CSS.

## Key Features ✨
### 1. Swiper Gallery
- Built with Swiper.js;

- Configurable via schema in the section settings:
- Number of visible slides
  - Space between slides
  - Enable/disable:
    - Pagination
    - Navigation arrows

- Fully responsive (desktop, tablet, mobile).

### 2. Image Filtering by Color Variant
- Displays only images related to the selected color variant;
- Works without page reload (based on change event on variant selector).

### 3. Dynamic Dropdown
- Data is pulled from a product metafield;
- Each option in the dropdown is treated as a separate value;
- The dropdown is not rendered if the field is empty.

## Installation 🛠️

### 1. Prerequisites
- Install [Node.js](https://nodejs.org/) (version 14 or higher) and npm.
- Install [Shopify CLI](https://shopify.dev/docs/themes/tools/cli/installation):
```bash
  npm install -g @shopify/cli
```
- Verify installation:
```bash
shopify --version
```
### 2. Clone the repository
```bash
git clone https://github.com/DariaRadtkina/shopify_theme_swiper_dropdown.git
```

```bash
cd shopify_theme_swiper_dropdown
```

### 3. Authentication

- Log in to your Shopify store to enable local development
```bash
shopify auth:login
```

### 4. Start the development server
```bash
shopify theme dev
```

## Known Issues ⚠️
- In the current implementation, the gallery includes a check using variantImages[initialVariantName] to ensure that products with a single image are displayed in full-screen mode. This enhancement provides an optimal viewing experience for single-image products, though it requires proper CSS styling to fully realize the full-screen effect.
