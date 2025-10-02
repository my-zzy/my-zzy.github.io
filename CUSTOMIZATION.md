# 🎨 Customization Guide

This guide will help you personalize your academic website with your own information, photos, and content.

## 📝 Step-by-Step Customization

### 1. Personal Information (index.html)

#### Update Basic Information
Find and replace these placeholders in `index.html`:

```html
<!-- Hero Section -->
<h1>Zhiyang Zhou</h1> <!-- Your name -->
<h2>PhD Student / Researcher</h2> <!-- Your title/position -->
<p class="hero-description">
    Welcome to my academic homepage. I am passionate about [Your Research Area] 
    and currently pursuing my PhD at [Your University].
</p>
```

#### Update Contact Information
```html
<!-- Social Links -->
<a href="mailto:your.email@university.edu" class="social-link">
<a href="https://scholar.google.com/citations?user=YOUR_ID" class="social-link">
<a href="https://github.com/my-zzy" class="social-link">
<a href="https://linkedin.com/in/yourprofile" class="social-link">
<a href="https://orcid.org/0000-0000-0000-0000" class="social-link">

<!-- Contact Section -->
<p>your.email@university.edu</p>
<p>Room XXX, Building Name<br>[University Name]<br>[City, State/Province]</p>
<p>+1 (XXX) XXX-XXXX</p>
```

### 2. Profile Photo

Replace the profile placeholder:
1. Add your professional photo as `profile.jpg` in the root directory
2. Update the HTML in the hero section:

```html
<!-- Replace this: -->
<div class="profile-placeholder">
    <i class="fas fa-user"></i>
    <p>Add Your Photo</p>
</div>

<!-- With this: -->
<img src="profile.jpg" alt="Your Name" class="profile-img">
```

**Photo Requirements:**
- Square aspect ratio (e.g., 500x500px)
- Professional headshot
- Good lighting and quality
- File formats: JPG, PNG, or WebP

### 3. About Section

#### Education
```html
<div class="education-item">
    <div class="education-degree">PhD in Computer Science</div>
    <div class="education-school">Stanford University</div>
    <div class="education-year">2020 - Present</div>
</div>
```

#### Research Description
Update the paragraph text with your actual research interests and background.

### 4. Research Areas

#### Update Research Items
```html
<div class="research-item">
    <div class="research-icon">
        <i class="fas fa-brain"></i> <!-- Choose appropriate icon -->
    </div>
    <h3>Machine Learning</h3> <!-- Your research area -->
    <p>Description of your research in this area.</p>
</div>
```

#### Icon Options (Font Awesome)
- `fas fa-brain` - AI/Machine Learning
- `fas fa-robot` - Robotics
- `fas fa-chart-line` - Data Science
- `fas fa-microscope` - Research/Lab work
- `fas fa-network-wired` - Networks
- `fas fa-code` - Programming/Software
- `fas fa-database` - Databases
- `fas fa-shield-alt` - Security/Cryptography

### 5. Publications

#### Add Your Papers
```html
<div class="publication-item">
    <h3>Your Paper Title Here</h3>
    <p class="authors"><strong>Your Name</strong>, Co-Author Name, Another Author</p>
    <p class="venue">Conference/Journal Name, Year</p>
    <div class="publication-links">
        <a href="link-to-paper.pdf" class="pub-link">Paper</a>
        <a href="github.com/yourrepo" class="pub-link">Code</a>
        <a href="slides.pdf" class="pub-link">Slides</a>
        <a href="dataset-link" class="pub-link">Dataset</a>
    </div>
</div>
```

#### Publication Order
- List publications in reverse chronological order (newest first)
- Bold your name in the author list
- Include full venue names and years

### 6. Teaching Experience

```html
<div class="teaching-item">
    <h3>Introduction to Machine Learning</h3>
    <p class="role">Teaching Assistant | Fall 2023</p>
    <p>Assisted with lectures, graded assignments, and held office hours for 150+ students.</p>
</div>
```

### 7. Color Scheme Customization

Edit `style.css` to change colors:

```css
/* Primary Colors */
:root {
    --primary-color: #3498db;    /* Blue */
    --secondary-color: #2c3e50;  /* Dark blue-gray */
    --accent-color: #667eea;     /* Purple-blue */
    --text-color: #333;          /* Dark gray */
    --light-bg: #f8f9fa;        /* Light gray background */
}
```

#### Popular Academic Color Schemes
1. **Classic Blue**: `#2c3e50`, `#3498db`, `#ecf0f1`
2. **Forest Green**: `#27ae60`, `#2c3e50`, `#ecf0f1`  
3. **Deep Purple**: `#8e44ad`, `#2c3e50`, `#ecf0f1`
4. **Warm Orange**: `#e67e22`, `#2c3e50`, `#ecf0f1`

### 8. Additional Sections (Optional)

#### Awards & Honors
```html
<section id="awards" class="section">
    <div class="container">
        <h2 class="section-title">Awards & Honors</h2>
        <div class="awards-list">
            <div class="award-item">
                <h3>Best Paper Award</h3>
                <p class="award-venue">International Conference on Machine Learning, 2023</p>
            </div>
        </div>
    </div>
</section>
```

#### News/Updates
```html
<section id="news" class="section bg-light">
    <div class="container">
        <h2 class="section-title">Recent News</h2>
        <div class="news-list">
            <div class="news-item">
                <span class="news-date">Oct 2025</span>
                <p>Paper accepted at NeurIPS 2025!</p>
            </div>
        </div>
    </div>
</section>
```

## 🚀 Deployment

### GitHub Pages Setup
1. Go to your repository settings
2. Navigate to "Pages" in the left sidebar
3. Under "Source", select "Deploy from a branch"
4. Choose "main" branch and "/ (root)" folder
5. Click "Save"
6. Your site will be available at `https://yourusername.github.io`

### Custom Domain (Optional)
1. Purchase a domain (e.g., `yourname.com`)
2. Add a `CNAME` file to your repository with your domain
3. Configure DNS settings with your domain provider
4. Enable HTTPS in GitHub Pages settings

## 📱 Testing

### Responsive Testing
Test your website on:
- Desktop (1920x1080, 1366x768)
- Tablet (768x1024, 1024x768)  
- Mobile (375x667, 414x896)

### Browser Testing
- Chrome
- Firefox  
- Safari
- Edge

### Performance Testing
Use tools like:
- Google PageSpeed Insights
- GTmetrix
- WebPageTest

## 🎯 SEO Optimization

### Meta Tags
Update the `<head>` section:
```html
<meta name="description" content="Zhiyang Zhou - PhD student and researcher specializing in machine learning and artificial intelligence.">
<meta name="keywords" content="machine learning, AI, research, PhD, computer science">
<meta name="author" content="Zhiyang Zhou">

<!-- Open Graph for social media -->
<meta property="og:title" content="Zhiyang Zhou - Academic Homepage">
<meta property="og:description" content="PhD student and researcher in machine learning">
<meta property="og:image" content="https://yourdomain.com/profile.jpg">
<meta property="og:url" content="https://yourdomain.com">
```

### Analytics (Optional)
Add Google Analytics:
```html
<!-- Add before closing </head> tag -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🔧 Troubleshooting

### Common Issues

**Website not loading on GitHub Pages:**
- Check that `index.html` is in the root directory
- Verify GitHub Pages is enabled in repository settings
- Wait 5-10 minutes after pushing changes

**Images not displaying:**
- Check file paths are correct
- Ensure images are committed to the repository
- Verify file extensions match (case-sensitive)

**Mobile menu not working:**
- Check that `script.js` is properly linked
- Verify JavaScript console for errors
- Test on different mobile devices

**Styling issues:**
- Check that `style.css` is properly linked
- Verify CSS syntax is correct
- Test on different browsers

### Getting Help
- Check browser developer console for errors
- Validate HTML at validator.w3.org
- Test CSS at jigsaw.w3.org/css-validator
- Open issues on GitHub for persistent problems

---

**Happy customizing! 🎉**

Remember to commit and push your changes to see them live on your GitHub Pages site.