# Read.cv Style Resume Template

A clean, fast-loading resume/profile template inspired by read.cv, designed for GitHub Pages deployment.

## Features

- **Fast Loading**: Optimized for minimal file size and quick page loads
- **Responsive**: Works perfectly on desktop and mobile devices
- **Accessible**: Semantic HTML with proper ARIA support and keyboard navigation
- **Clean Design**: Minimalist aesthetic inspired by read.cv
- **System Fonts**: Uses default system fonts for optimal performance
- **Smooth Animations**: Subtle hover effects and transitions
- **GitHub Pages Ready**: Deploy instantly to GitHub Pages

## Sections Included

- **Header**: Name, title, bio, and contact links
- **Experience**: Work history with company logos and descriptions
- **Education**: Academic background
- **Projects**: Portfolio projects with links
- **Skills**: Technology and skill tags
- **Awards**: Optional achievements section

## Quick Start

1. **Deploy to GitHub Pages**:
   - Fork this repository
   - Go to Settings → Pages
   - Select "Deploy from a branch" → main branch
   - Your site will be available at `https://yourusername.github.io/hines.digital`

2. **Customize Your Content**:
   - Edit `index.html` to replace the example content with your information
   - Update the `<title>` and meta description
   - Replace placeholder text with your actual details

## Customization Guide

### Personal Information
Replace these sections in `index.html`:

```html
<!-- Update header section -->
<h1>Your Name</h1>
<p class="subtitle">Your Professional Title</p>
<div class="bio">
    <p>Your bio here...</p>
</div>

<!-- Update contact links -->
<a href="mailto:your.email@example.com" class="contact-link">
```

### Experience Section
Add or modify experience entries:

```html
<article class="card">
    <div class="item-header">
        <div class="item-logo">CO</div> <!-- Company initials -->
        <div class="item-content">
            <h3 class="item-title">Job Title</h3>
            <p class="item-subtitle">Company Name</p>
            <p class="item-period">Start Date - End Date</p>
        </div>
    </div>
    <div class="item-description">
        <p>Job description and achievements...</p>
    </div>
</article>
```

### Projects Section
Add your projects:

```html
<article class="card">
    <h3 class="item-title">Project Name</h3>
    <p class="item-description">Project description...</p>
    <div class="project-links">
        <a href="https://project-demo.com" class="project-link">
            <span>🔗</span> Live Demo
        </a>
        <a href="https://github.com/user/repo" class="project-link">
            <span>🐙</span> GitHub
        </a>
    </div>
</article>
```

### Skills Section
Update your skills:

```html
<div class="skills-grid">
    <span class="skill-tag">Your Skill</span>
    <span class="skill-tag">Another Skill</span>
    <!-- Add more skills -->
</div>
```

## Styling Customization

The template uses inline CSS for maximum performance. To customize:

### Colors
Update these CSS variables in the `<style>` section:

```css
/* Main colors */
color: #333;           /* Text color */
background-color: #fff; /* Background */
color: #0066cc;        /* Link color */
border: 1px solid #eee; /* Border color */
```

### Typography
The template uses system fonts for optimal performance:

```css
font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Helvetica Neue', Arial, sans-serif;
```

### Layout
Adjust the container width:

```css
.container {
    max-width: 800px; /* Change this value */
}
```

## Performance Features

- **Inline CSS**: Eliminates additional HTTP requests
- **System Fonts**: No web font loading delays
- **Optimized Images**: Uses emoji icons instead of image files
- **Minimal JavaScript**: Zero JavaScript for maximum speed
- **Efficient CSS**: Minimal, optimized styles

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## Advanced Customization

### Adding Company Logos
Replace emoji placeholders with actual logos:

```html
<div class="item-logo">
    <img src="logo.png" alt="Company Logo" width="48" height="48">
</div>
```

### Custom Icons
Replace emoji icons with custom SVG icons for a more professional look.

### Additional Sections
Add new sections by following the existing pattern:

```html
<section class="section">
    <h2>Section Title</h2>
    <article class="card">
        <!-- Content here -->
    </article>
</section>
```

## License

This template is free to use and modify for personal and commercial projects.

## Contributing

Feel free to submit issues and pull requests to improve this template.

---

**Note**: This template is inspired by read.cv but is an independent implementation designed for self-hosting and customization.
