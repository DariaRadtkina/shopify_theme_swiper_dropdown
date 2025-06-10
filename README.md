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
- Works without page reload (based on change event on variant selector);
- Filtering is performed based on the alt text of images, which corresponds to the selected color variant.

### 3. Dynamic Dropdown
- Data is pulled from a product metafield;
- Each option in the dropdown is treated as a separate value;
- The dropdown is not rendered if the field is empty.

## Modified Files 📝
- sections/main-product.liquid: Houses the core Liquid logic for generating the Swiper gallery structure, including the initialization of the custom dropdown and integration with product data such as variants and metafields;
- snippets/custom-dropdown.liquid: Contains the Liquid implementation for the custom dropdown, handling the rendering of options from product metafields and ensuring the dropdown is hidden when no data is provided.

## Known Issues ⚠️
- In the current implementation, the gallery includes a check to ensure that products with a single image are displayed in full-screen mode. This enhancement provides an optimal viewing experience for single-image products.
