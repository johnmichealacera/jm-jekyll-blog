# JM Jekyll Blog

A personal blog built with Jekyll, featuring a clean and simple design for sharing thoughts, tutorials, and experiences in software development.

## 🚀 Features

- **Clean Design**: Simple and minimal layout focused on content
- **Author Support**: Multi-author blog with individual author pages
- **Markdown Posts**: Easy-to-write blog posts using Markdown
- **Responsive**: Mobile-friendly design
- **Fast Loading**: Static site generation for optimal performance

## 📁 Project Structure

```
jm-jekyll-blog/
├── _authors/          # Author profiles and information
├── _data/             # Site data and configuration
├── _includes/         # Reusable HTML components
├── _layouts/          # Page templates
├── _posts/            # Blog posts (Markdown files)
├── _sass/             # Sass stylesheets
├── _site/             # Generated site (Git ignored)
├── _tests/            # Test files
├── assets/            # Static assets (images, CSS, JS)
├── _config.yml        # Jekyll configuration
├── Gemfile            # Ruby dependencies
├── index.html         # Homepage
├── about.md           # About page
├── blog.html          # Blog listing page
└── staff.html         # Staff/authors page
```

## 🛠️ Setup & Installation

### Prerequisites

- Ruby (version 2.7 or higher)
- RubyGems
- Bundler gem

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd jm-jekyll-blog
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Serve the site locally**
   ```bash
   bundle exec jekyll serve
   ```

4. **Access your site**
   Open your browser and navigate to `http://localhost:4000`

## ✍️ Writing Posts

### Creating a New Post

1. Create a new Markdown file in the `_posts` directory
2. Use the following naming convention: `YYYY-MM-DD-title.md`
3. Add front matter at the top of your file:

```yaml
---
layout: post
title: "Your Post Title"
author: JM
date: 2024-03-16
---
```

4. Write your content using Markdown syntax

### Post Example

```markdown
---
layout: post
title: "Getting Started with Jekyll"
author: JM
---

# Getting Started with Jekyll

This is your first Jekyll post!

## Features

- Easy to use
- Markdown support
- Fast static site generation
```

## 👥 Managing Authors

Authors are managed in the `_authors` directory. Each author has their own Markdown file with front matter:

```yaml
---
name: JM
position: Software Developer
bio: Passionate about technology and sharing knowledge
---
```

## 🎨 Customization

### Configuration

Edit `_config.yml` to customize your site:

```yaml
collections:
  authors:
    output: true

defaults:
  - scope:
      path: ""
      type: "authors"
    values:
      layout: "author"
  - scope:
      path: ""
      type: "posts"
    values:
      layout: "post"
```

### Styling

- Sass files are located in `_sass/`
- CSS can be customized by modifying the stylesheets
- Assets (images, etc.) go in the `assets/` directory

## 🚀 Deployment

### GitHub Pages

1. Push your code to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Select source as "Deploy from a branch"
4. Choose your main branch
5. Your site will be available at `https://username.github.io/repository-name`

### Other Platforms

- **Netlify**: Connect your GitHub repo for automatic deployments
- **Vercel**: Import your repository for seamless deployment
- **GitLab Pages**: Similar to GitHub Pages but on GitLab

## 📝 Available Pages

- **Homepage** (`index.html`): Welcome message and introduction
- **Blog** (`blog.html`): List of all blog posts
- **About** (`about.md`): About page content
- **Staff** (`staff.html`): List of authors and contributors

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 📞 Contact

- **Author**: JM
- **Email**: [Your Email]
- **Website**: [Your Website]

## 🙏 Acknowledgments

- Built with [Jekyll](https://jekyllrb.com/)
- Inspired by clean, minimal blog designs
- Thanks to the Jekyll community for excellent documentation

---

**Happy Blogging!** 🎉
