# Overview

This is a personal portfolio website project called "CINEMATIC" - a static website showcasing personal information, projects, and blog posts. It's built as a learning project with HTML, CSS, and vanilla JavaScript, featuring a multi-page structure with consistent navigation and styling across all pages.

# Recent Changes

**November 22, 2025** - Fixed GitHub Pages CSS loading issue
- Changed all CSS and JavaScript file paths from absolute (`/style.css`) to relative (`style.css`) in index.html, blog.html, and portfolio.html
- Added `.nojekyll` file to repository root to bypass Jekyll processing on GitHub Pages
- **Rationale**: GitHub Pages hosts sites at `username.github.io/repo-name/`, so absolute paths were looking for files at the wrong location
- **Impact**: CSS now loads correctly on GitHub Pages deployment

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture

**Multi-Page Static Website**
- **Structure**: Traditional multi-page application with separate HTML files (index.html, portfolio.html, blog.html)
- **Rationale**: Simple, beginner-friendly approach suitable for a personal portfolio site without need for a build process or framework
- **Pros**: Easy to understand, no dependencies, fast loading, SEO-friendly
- **Cons**: Requires duplicating navigation and header markup across pages

**Component Pattern**
- **Header Component**: Reused across all pages with centered text overlay on header image
- **Navigation Bar**: Consistent three-link navigation (HOME, PORTFOLIO, BLOG) on every page
- **Layout Structure**: Uses wrapper divs (#page-container, #content-wrap) for consistent page layout

**Styling Approach**
- **CSS Strategy**: Single global stylesheet (style.css) for all pages
- **Positioning**: Combination of absolute positioning (header text overlay) and standard flow
- **Responsiveness**: Includes viewport meta tag for mobile compatibility

**Interactive Features**
- **Scroll-to-Top Button**: JavaScript-powered button that appears after scrolling 700px down the page
- **Implementation**: Uses vanilla JavaScript with window scroll event listener
- **Rationale**: Enhances user experience on longer pages without requiring external libraries

## Asset Management

**Image Organization**
- **Assets Folder**: Centralized assets directory for images
- **Header Images**: Stored in assets/header/ subdirectory
- **Image Attribution**: Documented in README for licensing compliance (public domain and Creative Commons)

**Favicon Support**
- **Implementation**: favicon2.ico linked in index.html only
- **Note**: Could be extended to other pages for consistency

# External Dependencies

**None** - This is a pure HTML/CSS/JavaScript project with no external libraries, frameworks, or third-party services.

**Browser APIs Used**:
- DOM API (document.getElementById, element.style)
- Window API (window.onscroll)
- Standard HTML5/CSS3 features

**Potential Future Integrations**:
- Google Fonts (currently uses system "open sans" font with fallback to sans-serif)
- YouTube video embeds (mentioned as extension option in README)
- Analytics services for tracking site visits