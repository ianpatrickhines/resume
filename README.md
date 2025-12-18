# Resume Template

A clean, fast-loading resume/profile template inspired by read.cv, designed for GitHub Pages deployment with YAML-based content management.

**[View Live Demo](https://ianpatrickhines.github.io/resume/)**

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

- **Header**: Name, title, bio, contact links, and optional CV link
- **Experience**: Work history with company logos, descriptions, location, and company URLs
- **Education**: Academic background (optional)
- **Side Projects**: Personal projects and explorations with links
- **Client Projects**: Professional portfolio projects with images and links (optional)
- **Speaking**: Conference talks and presentations (optional)
- **Features**: Media mentions and publications (optional)
- **Skills**: Technology and skill tags (optional)
- **Certifications**: Professional certifications and credentials (optional)
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

3. **Update Configuration**:
   - Edit `_config.yml` to update the URL and repository references to match your GitHub username

## Content Management

All content is managed through the `_data/resume.yml` file. This approach:

- **Safe**: Prevents accidental HTML structure breaks
- **User-friendly**: No need to understand HTML/CSS
- **Maintainable**: Clean separation of content and presentation
- **Version-controlled**: Easy to track content changes

### Complete YAML Schema

Here's the complete structure of the `_data/resume.yml` file:

```yaml
# Personal Information (Required)
personal:
  name: "Your Name"
  title: "Your Title/Role"
  bio: "Your bio description..."
  avatar: "👤"  # Emoji, initials, image URL, or local file
  cv_link: "https://example.com/cv"  # Optional

# Contact Information (Required)
contact:
  email: "your@email.com"
  linkedin: "https://linkedin.com/in/username"
  github: "https://github.com/username"
  twitter: "https://twitter.com/username"  # Optional
  website: "https://yoursite.com"  # Optional
  phone: "+1 (555) 123-4567"  # Optional

# Work Experience (Required)
experience:
  - company: "Company Name"
    logo: "CO"  # Emoji, initials, or image URL
    position: "Your Position"
    period: "2020 - Present"
    location: "City, State"  # Optional
    company_url: "https://company.com"  # Optional
    description: "Description of your role..."

# Education (Optional - controlled by settings.show_education)
education:
  - institution: "University Name"
    logo: "🎓"
    degree: "Degree Name"
    period: "2018 - 2020"
    description: "Optional description..."

# Side Projects (Optional)
side_projects:
  - title: "Project Title"
    year: "2024"
    description: "Project description..."
    url: "https://project.com"

# Client Projects (Optional)
client_projects:
  - name: "Project Name"
    year: "2024"
    description: "Project description..."
    url: "https://project.com"  # Optional
    image: "https://example.com/image.jpg"  # 200x100px
    links:
      - name: "Demo"
        url: "https://demo.com"
        icon: "🔗"

# Speaking (Optional)
speaking:
  - title: "Talk Title"
    event: "Conference Name"
    year: "2024"
    description: "Talk description..."
    url: "https://talk.com"

# Features (Optional)
features:
  - title: "Article Title"
    publication: "Publication Name"
    year: "2024"
    description: "Feature description..."
    url: "https://article.com"

# Skills (Optional)
skills:
  - "Skill 1"
  - "Skill 2"
  - "Skill 3"

# Certifications (Optional)
certifications:
  - title: "Certification Name"
    organization: "Organization"
    year: "2024"
    description: "Certification description..."

# Awards (Optional - controlled by settings.show_awards)
awards:
  - title: "Award Name"
    organization: "Organization"
    year: "2024"
    description: "Award description..."

# Settings (Required)
settings:
  show_awards: true  # Show/hide awards section
  show_education: true  # Show/hide education section
  theme_color: "#0066cc"  # Light theme color
  dark_theme_color: "#5aa3ff"  # Dark theme color (optional)
```

### Editing Your Resume

Simply edit the `_data/resume.yml` file with your information:

```yaml
# Personal Information
personal:
  name: "Jane Smith"
  title: "Senior Product Designer"
  bio: "Passionate designer with 8+ years creating user-centered digital experiences..."
  avatar: "👩‍💼"  # Emoji, initials, or image URL
  cv_link: "https://example.com/cv"  # Optional CV/portfolio link

# Contact Information
contact:
  email: "jane.smith@example.com"
  linkedin: "https://linkedin.com/in/janesmith"
  github: "https://github.com/janesmith"
  twitter: "https://twitter.com/janesmith"  # Optional
  website: "https://janesmith.design"  # Optional
  # phone: "+1 (555) 123-4567"  # Optional
```

### Photo Avatars

The avatar field supports multiple formats:
- **Emoji**: `"👩‍💼"` (displays as emoji)
- **Initials**: `"JS"` (displays as text)
- **Image URL**: `"https://example.com/photo.jpg"` (displays as round photo)
- **Local file**: `"assets/avatar.png"` (relative to repository root)

Image avatars are automatically styled as round, non-draggable photos that perfectly fill the avatar space.

## Advanced Customization

### Adding/Removing Sections

Edit `_data/resume.yml` to show/hide sections:

```yaml
settings:
  show_awards: true        # Show/hide awards section
  show_education: true     # Show/hide education section
  # All other sections (side_projects, client_projects, speaking,
  # features, skills) are shown if they exist in the YAML file
  theme_color: "#0066cc"   # Light theme accent color
  dark_theme_color: "#5aa3ff"  # Dark theme accent color (optional)
```

### Adding Experience

```yaml
experience:
  - company: "Google"
    logo: "GO"  # Can use emoji, initials, or image URL
    position: "Senior UX Designer"
    period: "2022 - Present"
    location: "San Francisco, CA"  # Optional
    company_url: "https://google.com"  # Optional
    description: "Lead design for mobile apps serving 50M+ users..."
```

### Adding Side Projects

```yaml
side_projects:
  - title: "Simple Resume Template"
    year: "2025"
    description: "A simple resume template for GitHub Pages."
    url: "https://github.com/username/resume"
```

### Adding Client Projects

```yaml
client_projects:
  - name: "Mobile App Redesign"
    year: "2024"
    description: "Complete redesign improving conversion by 40%..."
    url: "https://portfolio.com/project"  # Optional main project URL
    image: "https://via.placeholder.com/200x100"  # 200x100px image
    links:
      - name: "Case Study"
        url: "https://portfolio.com/project"
        icon: "📋"
      - name: "Live App"
        url: "https://app.com"
        icon: "📱"
```

### Adding Speaking Engagements

```yaml
speaking:
  - title: "Conference Talk Title"
    event: "Tech Conference 2024"
    year: "2024"
    description: "Spoke about innovative approaches to software development."
    url: "https://example.com/talk"
```

### Adding Media Features

```yaml
features:
  - title: "Feature Article Title"
    publication: "Tech Magazine"
    year: "2024"
    description: "Featured article about industry trends and innovations."
    url: "https://example.com/article"
```

### Adding Skills (Optional)

The skills section is optional and commented out by default. To enable it, uncomment and customize:

```yaml
skills:
  - "Figma"
  - "Sketch"
  - "User Research"
  - "Prototyping"
  - "JavaScript"
  - "React"
  # Add your skills here
```

### Adding Certifications

```yaml
certifications:
  - title: "Certified Kubernetes Administrator"
    organization: "Cloud Native Computing Foundation"
    year: "2024"
    description: "Demonstrates expertise in managing Kubernetes clusters."
  - title: "AWS Solutions Architect"
    organization: "Amazon Web Services"
    year: "2023"
    description: "Professional-level certification for designing AWS solutions."
```

### Analytics Tracking (Optional)

The template includes optional DataBuddy analytics integration. To enable it:

1. Get your client ID from [https://databuddy.cc](https://databuddy.cc)
2. Add your client ID in `_data/resume.yml`:

```yaml
settings:
  # ... other settings ...

  # DataBuddy Analytics Configuration
  databuddy_client_id: "your_client_id_here"

  # Optional: Configure specific tracking features (all default to true)
  databuddy_track_outgoing_links: true
  databuddy_track_interactions: true
  databuddy_track_engagement: true
  databuddy_track_scroll_depth: true
  databuddy_track_exit_intent: true
  databuddy_track_bounce_rate: true
  databuddy_track_web_vitals: true
  databuddy_enable_batching: true
```

**To disable analytics**: Leave the `databuddy_client_id` commented out (which is the default).

## Styling Customization

### Colors
Update theme colors in `_data/resume.yml`:

```yaml
settings:
  theme_color: "#0066cc"      # Light theme accent color
  dark_theme_color: "#5aa3ff" # Dark theme accent color (optional)
```

The resume includes comprehensive dark mode support:
- Automatic system preference detection
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
2. Install dependencies: `bundle install`
3. Serve locally: `bundle exec jekyll serve`
4. View at: `http://localhost:4000/resume`

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
