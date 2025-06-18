# Read.cv Style Resume Template

A clean, fast-loading resume/profile template inspired by read.cv, designed for GitHub Pages deployment with YAML-based content management.

## Features

- **Data-Driven Content**: All content managed through YAML files - no HTML editing required
- **Safe Content Updates**: Separate content from structure to prevent breaking changes
- **Jekyll Integration**: Built for GitHub Pages with Jekyll templating
- **Dark Mode Support**: Professional dark/light/auto theme toggle with WCAG compliant colors
- **Fast Loading**: Optimized for minimal file size and quick page loads
- **Responsive**: Works perfectly on desktop and mobile devices
- **Accessible**: Semantic HTML with proper ARIA support and keyboard navigation
- **Clean Design**: Minimalist aesthetic inspired by read.cv
- **System Fonts**: Uses default system fonts for optimal performance
- **Smooth Animations**: Subtle hover effects and transitions

## Sections Included

- **Header**: Name, title, bio, and contact links
- **Experience**: Work history with company logos and descriptions
- **Education**: Academic background (optional)
- **Projects**: Portfolio projects with links
- **Skills**: Technology and skill tags
- **Awards**: Optional achievements section

## Quick Start

1. **Deploy to GitHub Pages**:
   - Fork this repository
   - Go to Settings → Pages
   - Select "Deploy from a branch" → main branch
   - Your site will be available at `https://yourusername.github.io/resume`

2. **Customize Your Content**:
   - Edit `_data/resume.yml` to update all your information
   - No HTML editing required - all content is managed through the YAML file
   - The template automatically builds your resume from the data

## Content Management

All content is managed through the `_data/resume.yml` file. This approach:

- ✅ **Safe**: Prevents accidental HTML structure breaks
- ✅ **User-friendly**: No need to understand HTML/CSS
- ✅ **Maintainable**: Clean separation of content and presentation
- ✅ **Version-controlled**: Easy to track content changes

### Editing Your Resume

Simply edit the `_data/resume.yml` file with your information:

```yaml
# Personal Information
personal:
  name: "Jane Smith"
  title: "Senior Product Designer"
  bio: "Passionate designer with 8+ years creating user-centered digital experiences..."
  avatar: "👩‍💼"

# Contact Information  
contact:
  email: "jane.smith@example.com"
  linkedin: "https://linkedin.com/in/janesmith"
  github: "https://github.com/janesmith"
  # Add more as needed
```

## Advanced Customization

### Adding/Removing Sections

Edit `_data/resume.yml` to show/hide sections:

```yaml
settings:
  show_awards: false     # Hide awards section
  show_education: true   # Show education section
```

### Adding Experience

```yaml
experience:
  - company: "Google"
    logo: "GO"  # Can use emoji, initials, or image URL
    position: "Senior UX Designer"
    period: "2022 - Present"
    description: "Lead design for mobile apps serving 50M+ users..."
```

### Adding Projects

```yaml
projects:
  - name: "Mobile App Redesign"
    description: "Complete redesign improving conversion by 40%..."
    links:
      - name: "Case Study"
        url: "https://portfolio.com/project"
        icon: "📋"
      - name: "Live App"
        url: "https://app.com"
        icon: "📱"
```

### Updating Skills

```yaml
skills:
  - "Figma"
  - "Sketch"
  - "User Research"
  - "Prototyping"
  # Add your skills here
```

## Styling Customization

### Colors
Update theme colors in `_data/resume.yml`:

```yaml
settings:
  theme_color: "#0066cc"      # Light theme accent color
  dark_theme_color: "#5aa3ff" # Dark theme accent color (optional)
```

The resume includes comprehensive dark mode support:
- Theme toggle button (top-right corner) cycles between light/dark/auto modes
- System preference detection for seamless integration
- WCAG compliant contrast ratios for accessibility
- Smooth transitions with reduced-motion support

### Advanced Styling
For advanced styling changes, edit the CSS in `index.html`:

```css
/* Main colors */
color: #333;           /* Text color */
background-color: #fff; /* Background */
color: #0066cc;        /* Link color */
border: 1px solid #eee; /* Border color */
```

## Performance Features

- **Inline CSS**: Eliminates additional HTTP requests
- **System Fonts**: No web font loading delays
- **Optimized Images**: Uses emoji icons instead of image files
- **Jekyll Static Generation**: Pre-built HTML for maximum speed
- **Minimal JavaScript**: Zero JavaScript for maximum speed

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## Jekyll Development

To develop locally:

1. Install Jekyll: `gem install jekyll bundler`
2. Build site: `jekyll build`
3. Serve locally: `jekyll serve`
4. View at: `http://localhost:4000`

## GitHub Pages Compatibility

This template is fully compatible with GitHub Pages' Jekyll processing. Simply push changes to your repository and GitHub will automatically build and deploy your site.

## Migration from HTML Editing

If you were previously editing the HTML directly, simply copy your content to the appropriate sections in `_data/resume.yml`. The template will automatically generate the HTML structure.

## License

This template is free to use and modify for personal and commercial projects.

## Contributing

Feel free to submit issues and pull requests to improve this template.

---

**Note**: This template is inspired by read.cv but is an independent implementation designed for self-hosting and customization.
