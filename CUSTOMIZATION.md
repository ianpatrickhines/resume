# YAML Content Customization Guide

This file provides specific examples of how to customize your resume content using the `_data/resume.yml` file.

## Overview

All content is managed through `_data/resume.yml`. This approach:
- **Prevents HTML breaking**: Content is separate from structure
- **Easy to edit**: Simple YAML format, no HTML knowledge required
- **Version controlled**: Easy to track changes over time
- **Safe updates**: Template structure remains intact

## Personal Information

Update your basic information:

```yaml
personal:
  name: "Jane Smith"
  title: "Senior Product Designer"
  bio: "Passionate designer with 8+ years creating user-centered digital experiences. Led design teams at Fortune 500 companies, improving user satisfaction by 40%."
  avatar: "👩‍💼"  # Can be emoji or image URL
```

## Contact Information

Add your contact details:

```yaml
contact:
  email: "jane.smith@example.com"
  linkedin: "https://linkedin.com/in/janesmith"
  github: "https://github.com/janesmith"
  twitter: "https://twitter.com/janesmith"
  website: "https://janesmith.design"
  phone: "+1 (555) 123-4567"  # Optional
```

**Note**: Only include the platforms you want to display. Remove or comment out (#) any you don't want.

## Experience Section

Add your work history:

```yaml
experience:
  - company: "Google"
    logo: "🔵"  # Can be emoji, initials like "GO", or image URL
    position: "Senior Product Designer"
    period: "March 2022 - Present"
    description: "Lead design for Google Workspace mobile apps, improving user engagement by 35%. Manage a team of 4 designers and collaborate with engineering teams across 3 time zones."
  
  - company: "Airbnb"
    logo: "🏠"
    position: "Product Designer"
    period: "January 2020 - February 2022"
    description: "Designed core booking flow improvements that increased conversion rate by 28%. Led user research initiatives and established design system components."
```

## Education Section

Add your educational background:

```yaml
education:
  - institution: "Stanford University"
    logo: "🌲"  # Can be emoji, initials, or image URL
    degree: "Master of Science in Human-Computer Interaction"
    period: "2018 - 2020"
    description: "Specialized in user experience design and cognitive psychology. Thesis: 'Mobile Interface Optimization Through Behavioral Analysis'"
  
  - institution: "UC Berkeley"
    logo: "🐻"
    degree: "Bachelor of Arts in Psychology"
    period: "2014 - 2018"
    description: "Magna cum laude. Focus on cognitive science and design psychology."
```

## Projects Section

Showcase your work:

```yaml
projects:
  - name: "E-commerce Mobile App Redesign"
    description: "Complete redesign of a shopping app serving 2M+ users. Improved conversion rate by 28% and reduced checkout abandonment by 40%. Led user research, wireframing, and design system creation."
    links:
      - name: "Case Study"
        url: "https://janesmith.design/ecommerce-redesign"
        icon: "📋"
      - name: "Prototype"
        url: "https://figma.com/proto/project"
        icon: "🎨"
  
  - name: "AI-Powered Design Assistant"
    description: "Built a Figma plugin that uses machine learning to suggest design improvements. Used by 10,000+ designers worldwide. Featured in Figma's official blog."
    links:
      - name: "Figma Plugin"
        url: "https://figma.com/community/plugin/ai-assistant"
        icon: "🔌"
      - name: "GitHub"
        url: "https://github.com/janesmith/ai-design-assistant"
        icon: "🐙"
```

## Skills Section

List your technologies and skills:

```yaml
# For a Designer
skills:
  - "Figma"
  - "Sketch"
  - "Adobe Creative Suite"
  - "Prototyping"
  - "User Research"
  - "Design Systems"
  - "HTML/CSS"
  - "Accessibility"
  - "A/B Testing"
  - "Wireframing"

# For a Developer
skills:
  - "JavaScript"
  - "TypeScript"
  - "React"
  - "Vue.js"
  - "Node.js"
  - "Python"
  - "PostgreSQL"
  - "AWS"
  - "Docker"
  - "Git"
  - "REST APIs"
  - "GraphQL"
```

## Awards Section

Add recognition and achievements:

```yaml
awards:
  - title: "Design Excellence Award"
    organization: "Google"
    year: "2023"
    description: "Recognized for outstanding contributions to Google Workspace mobile experience and user satisfaction improvements."
  
  - title: "Top Designer Recognition"
    organization: "Dribbble"
    year: "2022"
    description: "Featured as one of the top 10 emerging designers on Dribbble with over 100K followers."
```

## Settings Configuration

Control which sections appear:

```yaml
settings:
  show_awards: true       # Set to false to hide awards section
  show_education: true    # Set to false to hide education section
  theme_color: "#d45087" # Change the accent color (links, hovers)
```

## Logo Options

For company/institution logos, you have several options:

```yaml
# Option 1: Emoji
logo: "🔵"

# Option 2: Initials
logo: "GO"  # For Google

# Option 3: Image URL (if you host images)
logo: "https://logo.clearbit.com/google.com"

# Option 4: Local image (place in assets folder)
logo: "/assets/logos/google.png"
```

## Professional Examples

### Tech Professional
```yaml
personal:
  name: "Alex Chen"
  title: "Full Stack Developer"
  bio: "Passionate full-stack developer with 6+ years building scalable web applications. Love turning complex problems into simple, elegant solutions."
  avatar: "👨‍💻"

contact:
  email: "alex.chen@email.com"
  linkedin: "https://linkedin.com/in/alexchen"
  github: "https://github.com/alexchen"

skills:
  - "JavaScript"
  - "Python"
  - "React"
  - "Django"
  - "PostgreSQL"
  - "AWS"
  - "Docker"
```

### Marketing Professional
```yaml
personal:
  name: "Sarah Johnson"
  title: "Digital Marketing Manager"
  bio: "Data-driven marketing professional specializing in growth hacking and conversion optimization. Increased revenue by 300% across multiple SaaS companies."
  avatar: "📊"

contact:
  email: "sarah.johnson@email.com"
  linkedin: "https://linkedin.com/in/sarahjohnson"
  website: "https://sarahmarketing.com"

skills:
  - "Google Analytics"
  - "A/B Testing"
  - "SEO/SEM"
  - "Content Strategy"
  - "Growth Hacking"
  - "Conversion Optimization"
```

## Tips for Great Content

1. **Be Specific**: Use numbers and metrics in descriptions
2. **Show Impact**: Focus on results and achievements
3. **Keep it Concise**: 1-2 sentences per description
4. **Use Action Words**: Led, built, improved, designed, etc.
5. **Update Regularly**: Keep information current

## Deployment

After editing `_data/resume.yml`:

1. Commit your changes to git
2. Push to your GitHub repository
3. GitHub Pages will automatically rebuild your site
4. Changes will be live within a few minutes

Your resume will automatically update with your new content while maintaining the clean design and structure!