# COALAB Website

This is the official website for the Computational and Applied Linguistics Laboratory (COALAB). The site is built using Jekyll and deployed via GitHub Pages.

## Website Structure

- **Home** (`index.html`) - Overview of the lab, research highlights, featured projects, latest news
- **Research** (`research.md`) - Detailed description of research areas and facilities
- **Projects** (`projects.md`) - Current and completed research projects
- **Publications** (`publications.md`) - List of publications by year
- **Team** (`team.md`) - Lab members including PI, postdocs, students
- **News** (`news.md`) - Lab updates, events, announcements
- **Contact & Join** (`contact.md`) - Contact information and opportunities to join the lab

## Development

### Prerequisites

- Ruby 2.5.0 or higher
- Bundler gem

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/Peter-awe/coalab-website.git
   cd coalab-website
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Run the development server:
   ```bash
   bundle exec jekyll serve
   ```

4. Open your browser to `http://localhost:4000`

### Building for Production

To build the site for production:

```bash
bundle exec jekyll build
```

The built site will be in the `_site` directory.

## Deployment

This site is configured for deployment on GitHub Pages. The site will automatically build and deploy when changes are pushed to the `main` branch.

### Custom Domain

The site is configured to use the custom domain `coalab.org`. DNS settings should point to GitHub Pages servers.

## Adding Content

### Adding a New Page

1. Create a new Markdown file in the root directory (e.g., `newpage.md`)
2. Add front matter:
   ```yaml
   ---
   layout: default
   title: Page Title
   permalink: /newpage/
   ---
   ```
3. Add content below the front matter

### Adding a Blog Post

1. Create a new Markdown file in the `_posts` directory with filename format `YYYY-MM-DD-title.md`
2. Add front matter:
   ```yaml
   ---
   layout: post
   title: "Post Title"
   date: YYYY-MM-DD HH:MM:SS +/-TTTT
   categories: [category1, category2]
   ---
   ```
3. Add content below the front matter

### Adding a Team Member

1. Create a new Markdown file in the `_team` directory
2. Add front matter:
   ```yaml
   ---
   layout: team
   name: "Full Name"
   position: "Position"
   image: "/assets/img/team/filename.jpg"
   ---
   ```
3. Add bio content below the front matter

## Customization

### Styles

CSS files are located in `assets/css/`:
- `style.css` - Main stylesheet

### JavaScript

JavaScript files are located in `assets/js/`:
- `main.js` - Main JavaScript file

### Layouts

Layout templates are located in `_layouts/`:
- `default.html` - Default layout for all pages
- Additional layouts can be added as needed

## License

© 2025 COALAB - Computational and Applied Linguistics Laboratory. All rights reserved.

The website content is proprietary and should not be reproduced without permission.

## Contact

For website issues or updates, contact the lab at [contact@coalab.org](mailto:contact@coalab.org).
