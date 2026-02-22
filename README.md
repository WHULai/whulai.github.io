# Personal Academic Homepage

This is the source code of my personal academic homepage, built based on the [Minimal Light theme](https://github.com/yaoyao-liu/minimal-light) by [Yaoyao Liu](https://github.com/yaoyao-liu).

**Live Site:** https://whulai.github.io

## Project Overview

This academic homepage showcases my research, projects, and academic achievements as a Robotics Engineering student at Wuhan University. The site is designed to provide a clean and professional presentation of my academic profile with the following features:

- **Professional academic homepage design** - Clean and elegant layout suitable for academic profiles
- **Publications showcase** - Display research papers with images, links, and citation information
- **Research interests** - Detailed descriptions of research areas and focus
- **Projects and achievements** - Highlight academic projects, awards, and skills
- **Responsive design** - Mobile-friendly layout that works on all devices
- **Dark mode support** - Automatic dark theme based on system preferences
- **Optimized for academic networking** - Integration with ORCID, GitHub, and other academic platforms

## Project Structure

```
.
├── _data/                    # Data files (publications, etc.)
├── _includes/                # Reusable markdown includes
├── _layouts/                 # HTML templates
├── _sass/                    # Stylesheets
├── assets/                   # Static assets (images, files)
│   └── img/                  # Profile pictures and publication images
├── .gitignore               # Git ignore rules
├── CNAME                    # Custom domain configuration
├── Gemfile                  # Ruby dependencies
├── _config.yml              # Jekyll configuration
├── index.md                 # Main homepage content
└── README.md               # This file
```

## Quick Start

### Prerequisites

- Ruby (version 3.0 or higher recommended)
- Bundler gem
- Jekyll

Local preview requires Jekyll to be installed. The project uses Ruby version management via rbenv for an isolated environment.

### Local Development and Preview

To preview the site locally, use the Jekyll development server:

```bash
# Navigate to the project directory
cd whulai.github.io

# Start the Jekyll server
eval "$(rbenv init -)" && bundle exec jekyll serve
```

The site will be available at **http://localhost:4000**. The server automatically rebuilds when files are changed.

To stop the server, press `Ctrl + C` in the terminal.

### Building Static Files

To generate static HTML files without starting the server:

```bash
eval "$(rbenv init -)" && bundle exec jekyll build
```

The generated files will be in the `_site` directory and can be deployed to any web server.

## Configuration

### Personal Information

Edit `_config.yml` to update:
- Name, position, and affiliation
- Contact information (email, ORCID)
- Social media and academic profile links
- Profile and favicon images
- Theme settings (dark mode, font selection)

### Content Management

- **index.md**: Main homepage content including About Me, Education, Research Interests, Projects, and Skills
- **_data/publications.yml**: Add or update publications with titles, authors, links, and images
- **_includes/**: Modify included sections (publications display format)
- **assets/img/**: Add profile pictures and publication images

### Styling

- Edit `_sass/minimal-light.scss` to customize the appearance
- The theme supports both Serif and Sans Serif fonts (configured in `_config.yml`)
- Dark mode can be enabled/disabled via the `auto_dark_mode` setting

## Deployment

### GitHub Pages (Recommended)

This site is configured for automatic deployment via GitHub Pages. Simply push changes to the repository, and GitHub Pages will build and serve the site at https://whulai.github.io

### Custom Domain

The CNAME file is configured for custom domain support. Update this file if using a custom domain instead of the default GitHub Pages URL.

## Acknowledgments

This project is built upon the excellent [Minimal Light theme](https://github.com/yaoyao-liu/minimal-light) created by [Yaoyao Liu](https://github.com/yaoyao-liu), which is licensed under the Creative Commons Zero v1.0 Universal License.

I would like to express my sincere gratitude to:
- **Yaoyao Liu** for creating the elegant Minimal Light theme that provides a solid foundation for academic homepages
- The Jekyll community for the excellent static site generator
- GitHub for providing the GitHub Pages hosting service

The Minimal Light theme is inspired by:
- [pages-themes/minimal](https://github.com/pages-themes/minimal)
- [orderedlist/minimal](https://github.com/orderedlist/minimal)
- [al-folio](https://github.com/alshedivat/al-folio)

## License

This project inherits the same license as the Minimal Light theme: Creative Commons Zero v1.0 Universal License.

## Contact

For questions or suggestions regarding this website:
- GitHub Issues: https://github.com/WHULai/whulai.github.io/issues
- Email: lai-wei@whu.edu.cn
