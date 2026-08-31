# Blanket Statement - Hugo Starter Blog

A modern, fast, and responsive Hugo starter blog styled after [blanketstatementproject.com](https://blanketstatementproject.com/).

## Features

- **Exact Design & Styling**: Custom responsive landing page & blog matching the Blanket Statement visual aesthetic (Lato typography, signature `#367b81` teal / `#263366` navy palette, masthead hero banner, image showcases, and CTA).
- **All Assets Included**: Logo (`Blanket-Statement-Logo.png`), showcase imagery (`yarn-logo.jpg`, `knitted-squares.jpg`, `balls-of-yarn.jpg`), masthead background (`bg-masthead.jpg`), Bootstrap, FontAwesome 5 (with webfonts), Simple Line Icons, and Bluesky SVG branding.
- **Full Blog Architecture**:
  - **Homepage**: Hero masthead, 3-row image showcase, latest blog posts cards, and call-to-action banner.
  - **Blog List**: Filterable blog archive with sidebar (categories, recent posts, tag cloud, about widget) and pagination.
  - **Single Post**: Featured image, breadcrumbs, reading time, publication date, author bio box, previous/next article navigation, and markdown formatting.
  - **Taxonomies**: Tag and category index and archive pages.
  - **Static Pages**: About and Contact pages.
- **Modern Hugo Ready**: Configured for Hugo v0.128+ / v0.154+ using `hugo.toml`.

## Getting Started

### 1. Start the Local Development Server
Run the Hugo development server with drafts enabled:
```bash
hugo server -D
```
Open [http://localhost:1313/](http://localhost:1313/) in your web browser.

### 2. Create a New Blog Post
Create a new post using the built-in archetype:
```bash
hugo new posts/my-new-post.md
```
This generates frontmatter with default categories, tags, author, and image placeholders in `content/posts/my-new-post.md`.

### 3. Build the Production Site
Compile the static HTML, CSS, and assets into the `public/` folder:
```bash
hugo --gc --minify
```

## Directory Structure

```text
├── archetypes/       # Templates for new posts and pages
├── content/          # Markdown content
│   ├── about.md      # About page
│   ├── contact.md    # Contact page
│   └── posts/        # Blog articles
├── layouts/          # HTML templates & partials
│   ├── _default/     # Base layout, list, single, terms
│   ├── page/         # Single page layout
│   ├── partials/     # Nav, masthead, CTA, footer, sidebar, post card, pagination
│   ├── posts/        # Custom post layouts
│   └── index.html    # Homepage layout
├── static/           # Static assets
│   ├── css/          # landing-page.min.css & custom.css
│   ├── img/          # Logo and photos from blanketstatementproject.com
│   └── vendor/       # Bootstrap, FontAwesome, Simple Line Icons, jQuery
├── hugo.toml         # Site configuration
└── README.md
```

## Customization

You can edit `hugo.toml` to customize:
- `title`, `tagline`, `headline`, and `description`
- `[params.social]` links (Bluesky, Instagram, Twitter, Facebook, GitHub)
- `[params]` email (`cta_email`), copyright, and credit links
- Menu navigation items under `[[menu.main]]`
