# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the Lū'au Bay Website project - an educational Future Fiction Academy (FFA) lab project focused on "Poly Romance - Small Town" research and development. The repository contains a comprehensive single-page website showcasing the fictional island setting of Lū'au Bay, complete with character profiles, locations, and romance-themed content.

## Project Structure

### Core Files
- **`index.html`**: Complete single-page website with embedded CSS and JavaScript
- **Character Assets**: PNG files for main characters stored in root directory
- **Generated Images**: Romance-style artwork in `generated-images/romance-style/`

### Website Architecture

The website is a fully self-contained HTML file featuring:

#### CSS Architecture
- **Responsive Grid System**: Uses CSS Grid for character cards, locations, and gallery layouts
- **Color Palette**: Hawaiian-inspired colors (teal #1a535c, coral #ff6b6b, sunshine #ffd93d)
- **Animation System**: Floating animations, scroll effects, and hover transitions
- **Theme Elements**: Romance-focused gradients, backdrop filters, and tropical aesthetics

#### JavaScript Features
- **Scroll Navigation**: Dynamic navbar changes and smooth scrolling
- **Image Gallery System**: Lazy loading with 30-second timeout and error handling
- **Interactive Elements**: Character card animations and scroll-triggered animations
- **Intersection Observer**: Performance-optimized scroll animations with 0.1 threshold
- **Gallery Loading**: Dynamic image creation with fallback error messages

#### Content Sections
1. **Hero Section**: Animated title with Hawaiian motto "E hoʻokahi ka puana"
2. **About Section**: Grid layout explaining the setting's polyamory-friendly culture
3. **Characters Section**: Interactive cards for 5 main characters with image fallbacks
4. **Locations Section**: 6 romantic locations with background images
5. **Events Section**: Timeline of town traditions and festivals
6. **Gallery Section**: Dynamic image loading from generated artwork
7. **Footer**: Animated whale element

## Image Asset Management

### Character Images
- Stored in root directory (e.g., `Character - Coral.png`)
- Circle-cropped version available (`Character-Auntie-Mahina-Circle.png`)
- JavaScript includes fallback emoji when images fail to load

### Generated Artwork
All stored in `generated-images/romance-style/`:
- Location backgrounds: `driftwood-inn.png`, `sirens-pool.png`, etc.
- Scenic artwork: `whale-tail-sunset.png`, `sharing-table-sunset.png`
- Overview image: `luau-bay-overview.png` (used as hero background)

## Development Context

This is a static website with no build process, package managers, or external dependencies. The entire application is contained within a single HTML file with embedded styles and scripts.

### Development Commands
- **Local Preview**: Simply open `index.html` in any modern web browser
- **No Build Process**: No npm, webpack, or other build tools required
- **Live Deployment**: Project is hosted via GitHub Pages at https://blossomz37.github.io/luau-bay-website/

### File Architecture
- **Single File Application**: All HTML, CSS (894 lines), and JavaScript are embedded in `index.html`
- **Image Optimization**: JPEG versions provide 75-77% size reduction from original PNGs
- **Asset Organization**: Generated images stored in `generated-images/romance-style/` with both JPG and PNG formats

### Image Loading Strategy
- Uses lazy loading (`loading="lazy"`) for performance
- Implements loading states with CSS animations
- Graceful fallbacks for missing images
- Error handling displays fallback content

### Performance Considerations
- Self-contained architecture minimizes HTTP requests
- Intersection Observer for efficient scroll animations
- CSS animations use transforms for smooth performance
- Responsive design with mobile-first approach

## Project Purpose

Educational project for FFA (Future Farmers of America) lab work, specifically Lab 3 focusing on "Poly Romance - Small Town" research and development. The website serves as a comprehensive world-building showcase for the fictional Lū'au Bay setting, emphasizing themes of ethical non-monogamy, community, and Hawaiian-inspired culture.