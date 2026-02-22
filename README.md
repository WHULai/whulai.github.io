# Personal Academic Homepage

This is the source code of my personal academic homepage, built based on the [Minimal Light theme](https://github.com/yaoyao-liu/minimal-light) by [Yaoyao Liu](https://github.com/yaoyao-liu).

**Live Site:** https://whulai.github.io

## About This Project

This academic homepage showcases my research, projects, and academic achievements as a Robotics Engineering student at Wuhan University. The site is designed to provide a clean and professional presentation of my academic profile.

## Features

- Clean and elegant academic homepage design
- Jekyll-based static site with GitHub Pages deployment
- Responsive design for mobile devices
- Publications showcase with links to papers and code
- Research interests and project highlights
- Skills and awards section
- Dark mode support

## Project Structure

```
.
├── _data/                    # Data files (publications, etc.)
├── _includes/                # Reusable markdown includes
├── _layouts/                 # HTML templates
├── _sass/                    # Stylesheets
├── assets/                   # Static assets (images, files)
├── .gitignore               # Git ignore rules
├── CNAME                    # Custom domain configuration
├── Gemfile                  # Ruby dependencies
├── _config.yml              # Jekyll configuration
├── index.md                 # Main homepage content
└── README.md               # This file
```

## Getting Started

### Prerequisites

- Ruby (version 2.5 or higher)
- Bundler gem
- Jekyll

### Local Development

1. **Clone the repository:**
   ```bash
   git clone git@github.com:WHULai/whulai.github.io.git
   cd whulai.github.io
   ```

2. **Install dependencies:**
   ```bash
   bundle install
   bundle add webrick
   ```

3. **Run the development server:**
   ```bash
   bundle exec jekyll serve
   ```

4. **Preview the site:**
   Open your browser and navigate to http://localhost:4000

5. **Build static files:**
   Static HTML files will be generated in the `_site` directory.

### GitHub Pages Deployment

This site is configured to automatically deploy via GitHub Pages. Simply push changes to the repository, and GitHub Pages will build and serve the site.

## Customization

### Configuration

Edit `_config.yml` to update:
- Personal information (name, position, affiliation)
- Contact details and links
- Images (avatar, favicon)
- Theme settings (dark mode, font)

### Content

- **index.md:** Main homepage content, research interests, projects, and awards
- **_data/publications.yml:** Add or update publications
- **_includes/:** Modify included sections (publications, services)
- **assets/img/:** Add profile picture and other images

### Styling

Edit `_sass/minimal-light.scss` to customize the appearance of the site.

## Deployment

### Using GitHub Pages (Recommended)

The site automatically deploys to GitHub Pages when changes are pushed to the main branch. The site is available at: https://whulai.github.io

### Using Docker (Alternative Preview Method)

For an isolated environment, you can use Docker to preview the site:

1. **Build and run with Docker:**
   ```bash
   docker run --rm -v "$PWD":/usr/src/app -p "4000:4000" -it ruby:3.1 bash
   ```

2. **Inside the container:**
   ```bash
   cd /usr/src/app
   bundle install
   bundle exec jekyll serve --host 0.0.0.0 --port 4000
   ```

3. **Preview:**
   Open http://localhost:4000 in your browser

### Local Jekyll Installation

Alternatively, you can install Jekyll locally following the [official Jekyll installation guide](https://jekyllrb.com/docs/installation/).

## Acknowledgments

This project is based on the [Minimal Light theme](https://github.com/yaoyao-liu/minimal-light) created by [Yaoyao Liu](https://github.com/yaoyao-liu), which is licensed under the Creative Commons Zero v1.0 Universal License.

I would like to express my sincere gratitude to:
- [Yaoyao Liu](https://github.com/yaoyao-liu) for creating the elegant Minimal Light theme
- The Jekyll community for the excellent static site generator
- GitHub for providing the Pages hosting service

The Minimal Light theme itself is inspired by:
- [pages-themes/minimal](https://github.com/pages-themes/minimal)
- [orderedlist/minimal](https://github.com/orderedlist/minimal)
- [al-folio](https://github.com/alshedivat/al-folio)

## License

This project inherits the same license as the Minimal Light theme: Creative Commons Zero v1.0 Universal License.

## Contact

For questions or suggestions regarding this website, please contact:
- Email: weilai@weilai.group
- GitHub: https://github.com/WHULai

## Quick Preview Guide

### Easiest Method: Docker

```bash
# Run in the project directory
docker run --rm -v "$PWD":/site -p 4000:4000 -it starefossen/github-pages
```

Then open http://localhost:4000 in your browser.

### Alternative Method: Local Jekyll

```bash
# Install dependencies
bundle install
bundle add webrick

# Run server
bundle exec jekyll serve

# View at http://localhost:4000
```

### Build Static Files

```bash
bundle exec jekyll build
# HTML files will be in _site directory
```
