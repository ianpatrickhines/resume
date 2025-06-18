# Customization Examples

This file provides specific examples of how to customize the template with your own content.

## Header Section Customization

Replace the placeholder header with your information:

```html
<!-- Before -->
<h1>Your Name</h1>
<p class="subtitle">Your Professional Title</p>

<!-- After -->
<h1>Jane Smith</h1>
<p class="subtitle">Senior Product Designer</p>
```

## Contact Links

Update contact information:

```html
<!-- Email -->
<a href="mailto:jane.smith@example.com" class="contact-link">

<!-- LinkedIn -->
<a href="https://linkedin.com/in/janesmith" class="contact-link">

<!-- GitHub -->
<a href="https://github.com/janesmith" class="contact-link">

<!-- Portfolio Website -->
<a href="https://janesmith.design" class="contact-link">
    <span>🌐</span>
    Portfolio
</a>
```

## Experience Section

Add your work history:

```html
<article class="card">
    <div class="item-header">
        <div class="item-logo">GO</div> <!-- Google -->
        <div class="item-content">
            <h3 class="item-title">Senior Product Designer</h3>
            <p class="item-subtitle">Google</p>
            <p class="item-period">March 2022 - Present</p>
        </div>
    </div>
    <div class="item-description">
        <p>Lead design for Google Workspace mobile apps, improving user engagement by 35%. Manage a team of 4 designers and collaborate with engineering teams across 3 time zones.</p>
    </div>
</article>
```

## Skills Customization

Update with your specific skills:

```html
<!-- For a Developer -->
<div class="skills-grid">
    <span class="skill-tag">JavaScript</span>
    <span class="skill-tag">React</span>
    <span class="skill-tag">Node.js</span>
    <span class="skill-tag">Python</span>
    <span class="skill-tag">AWS</span>
    <span class="skill-tag">Docker</span>
    <span class="skill-tag">PostgreSQL</span>
    <span class="skill-tag">Git</span>
</div>

<!-- For a Designer -->
<div class="skills-grid">
    <span class="skill-tag">Figma</span>
    <span class="skill-tag">Sketch</span>
    <span class="skill-tag">Adobe Creative Suite</span>
    <span class="skill-tag">Prototyping</span>
    <span class="skill-tag">User Research</span>
    <span class="skill-tag">Design Systems</span>
    <span class="skill-tag">HTML/CSS</span>
    <span class="skill-tag">Accessibility</span>
</div>
```

## Projects Section

Showcase your best work:

```html
<article class="card">
    <h3 class="item-title">E-commerce Mobile App Redesign</h3>
    <p class="item-description">Complete redesign of a shopping app serving 2M+ users. Improved conversion rate by 28% and reduced checkout abandonment by 40%. Led user research, wireframing, and design system creation.</p>
    <div class="project-links">
        <a href="https://dribbble.com/shots/project" class="project-link" target="_blank" rel="noopener">
            <span>🎨</span>
            Design
        </a>
        <a href="https://apps.apple.com/app/project" class="project-link" target="_blank" rel="noopener">
            <span>📱</span>
            App Store
        </a>
    </div>
</article>
```

## Education Section

Add your educational background:

```html
<article class="card">
    <div class="item-header">
        <div class="item-logo">MIT</div>
        <div class="item-content">
            <h3 class="item-title">Master of Science in Computer Science</h3>
            <p class="item-subtitle">Massachusetts Institute of Technology</p>
            <p class="item-period">2018 - 2020</p>
        </div>
    </div>
    <div class="item-description">
        <p>Specialized in Human-Computer Interaction and Machine Learning. Thesis: "Improving Mobile App Usability Through AI-Driven Interface Adaptation"</p>
    </div>
</article>
```

## Color Scheme Customization

To change the color scheme, update these CSS values:

```css
/* Professional Blue Theme */
a { color: #0066cc; }
a:hover { color: #004499; }
.contact-link:hover { background-color: #f8f9ff; }

/* Warm Theme */
a { color: #d45087; }
a:hover { color: #b73e6f; }
.contact-link:hover { background-color: #fdf8fa; }

/* Dark Mode Theme */
body { background-color: #1a1a1a; color: #e0e0e0; }
.card { background: #2d2d2d; border-color: #404040; }
a { color: #66b3ff; }
```

## Company Logo Integration

Replace emoji placeholders with actual company logos:

```html
<!-- Option 1: Image -->
<div class="item-logo">
    <img src="https://logo.clearbit.com/google.com" alt="Google" width="32" height="32">
</div>

<!-- Option 2: SVG Icon -->
<div class="item-logo">
    <svg width="32" height="32" viewBox="0 0 24 24">
        <!-- SVG path here -->
    </svg>
</div>

<!-- Option 3: Font Icon (if using icon font) -->
<div class="item-logo">
    <i class="fab fa-google"></i>
</div>
```

## Adding New Sections

To add custom sections like Publications or Volunteering:

```html
<!-- Publications Section -->
<section class="section">
    <h2>Publications</h2>
    <article class="card">
        <h3 class="item-title">The Future of Mobile Design</h3>
        <p class="item-subtitle">UX Magazine • December 2023</p>
        <p class="item-description">An exploration of emerging design patterns in mobile interfaces and their impact on user experience.</p>
        <div class="project-links">
            <a href="#" class="project-link" target="_blank" rel="noopener">
                <span>📖</span>
                Read Article
            </a>
        </div>
    </article>
</section>

<!-- Volunteering Section -->
<section class="section">
    <h2>Volunteering</h2>
    <article class="card">
        <div class="item-header">
            <div class="item-logo">❤️</div>
            <div class="item-content">
                <h3 class="item-title">UX Mentor</h3>
                <p class="item-subtitle">Design Buddies Community</p>
                <p class="item-period">2021 - Present</p>
            </div>
        </div>
        <div class="item-description">
            <p>Mentor junior designers transitioning into UX. Provide portfolio reviews, career guidance, and technical workshops for 50+ mentees.</p>
        </div>
    </article>
</section>
```

## Performance Tips

1. **Optimize Images**: Use WebP format and compress images
2. **Minimize Custom Fonts**: Stick to system fonts for best performance
3. **Compress CSS**: Remove unused styles when customizing
4. **Use CDN**: Host images on a CDN for faster loading

## GitHub Pages Setup

1. Enable GitHub Pages in repository settings
2. Choose "Deploy from a branch" → main
3. Your site will be live at `https://username.github.io/repository-name`
4. Custom domain can be configured in Settings → Pages