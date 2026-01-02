# Site Customization Log - 2026-01-02

Summary of changes made to the site configuration, layout, and styling.

## 1. Stock Photos Page
Grouped individual stock photo links into a dedicated page to declutter the sidebar.

- **New Page**: `stock-photos.md`
- **Config Update**: Updated `_config.yml` to link to `/stock-photos/`

## 2. Header Title Font (Parisienne)
Changed the site header "Compassute" to use the **Parisienne** font.

- **Font Link**: Added to `_includes/head/custom.html`
- **Forced Style**: Added `<style>` block in `_includes/head/custom.html` to guarantee application.
  ```html
  <style>
    .site-title, .site-title a {
      font-family: 'Parisienne', cursive !important;
      font-weight: 400 !important;
    }
  </style>
  ```
- **SCSS**: Also updated `assets/css/main.scss`, though the HTML injection is the primary enforcement method.

## 3. Dark Theme & Custom CSS
Resolved an issue where creating `assets/css/main.scss` broke the dark theme.

- **Solution**: Explicitly imported the dark skin in `assets/css/main.scss`.
  ```scss
  @import "minimal-mistakes/skins/dark";
  @import "minimal-mistakes";
  ```

## 4. Default Layout & Header Image
Configured the default layout to `single` and set a global header image.

- **Config**: Added `defaults` section to `_config.yml`.
  ```yaml
  defaults:
    - scope:
        path: ""
      values:
        layout: "single"
        header:
          image: "/assets/images/chausudake_panorama_mini.jpg"
  ```
