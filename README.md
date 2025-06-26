# Richard Cole McKain - Digital Portfolio

A modern, responsive portfolio website showcasing Richard Cole McKain's work as a Freelance IT Technician and Mobile Application Developer. Built with HTML, CSS, and JavaScript.

## 🌟 Features

- **Modern Design**: Clean, professional design with smooth animations
- **Fully Responsive**: Works perfectly on desktop, tablet, and mobile devices
- **Interactive Elements**: Smooth scrolling, hover effects, and dynamic content
- **Contact Form**: Functional contact form with service selection and validation
- **Dark Mode Support**: Automatically adapts to user's system preferences
- **Performance Optimized**: Fast loading with lazy loading and optimized assets
- **SEO Friendly**: Proper meta tags and semantic HTML structure

## 📁 Project Structure

```
Digital Portfolio/
├── index.html          # Main HTML file
├── css/
│   ├── style.css       # Main stylesheet
│   └── responsive.css  # Responsive design styles
├── js/
│   └── main.js         # JavaScript functionality
├── images/             # Image assets (create this folder)
├── assets/             # Additional assets (create this folder)
└── README.md           # This file
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A web server (optional, for local development)

### Installation

1. **Clone or Download** the project files to your local machine

2. **Open the website**:
   - **Option 1**: Double-click `index.html` to open in your browser
   - **Option 2**: Use a local server for better development experience

### Local Development Server

For the best development experience, use a local server:

#### Using Python (if installed):
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

#### Using Node.js (if installed):
```bash
# Install http-server globally
npm install -g http-server

# Run the server
http-server
```

#### Using PHP (if installed):
```bash
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## 🎨 Customization

### Personal Information

Update the following sections in `index.html`:

1. **Hero Section** (lines ~50-60):
   ```html
   <h1 class="hero-title">Hi, I'm <span class="highlight">Richard Cole McKain</span></h1>
   <p class="hero-subtitle">Freelance IT Technician & Mobile Application Developer</p>
   ```

2. **About Section** (lines ~120-140):
   ```html
   <p>I'm a passionate IT professional and software developer with a strong foundation in both technical support and mobile application development...</p>
   ```

3. **Contact Information** (lines ~280-290):
   ```html
   <span>RichCMckain@gmail.com</span>
   <span>(209) 761-7030</span>
   ```

### Projects

The portfolio includes four main project categories:

1. **Cross-Platform Mobile Applications** - iOS and Android development
2. **AI Chatbot Development** - OpenAI API and Botpress integration
3. **IT Automation Solutions** - Python-based automation
4. **Cybersecurity Analysis** - IAM and security training

Add your specific projects by updating the project cards in the Projects section (around line 180):

```html
<div class="project-card">
    <div class="project-image">
        <div class="project-placeholder">
            <i class="fas fa-mobile-alt"></i>
        </div>
    </div>
    <div class="project-content">
        <h3>Your Project Name</h3>
        <p>Project description goes here...</p>
        <div class="project-tech">
            <span class="tech-tag">iOS</span>
            <span class="tech-tag">React Native</span>
        </div>
        <div class="project-links">
            <a href="#" class="project-link"><i class="fab fa-apple"></i> App Store</a>
            <a href="#" class="project-link"><i class="fab fa-google-play"></i> Play Store</a>
        </div>
    </div>
</div>
```

### Skills

The portfolio is organized into three main skill categories:

1. **Mobile Development** - iOS Development, React Native, Cross-Platform Development, App Store Deployment
2. **IT & System Administration** - Hardware Repair, System Installation, Data Backup & Recovery, Software Upgrades
3. **Programming & Automation** - Python, API Integration, Git Version Control, AI/ML Integration

Update your skills in the Skills section (around line 220):

```html
<div class="skill-item">
    <span class="skill-name">Your Skill</span>
    <div class="skill-bar">
        <div class="skill-progress" style="width: 85%"></div>
    </div>
</div>
```

### Colors and Styling

The main color scheme is defined in `css/style.css`. Key color variables:

- Primary gradient: `#667eea` to `#764ba2`
- Accent color: `#ffd700` (gold)
- Text colors: `#2d3748`, `#4a5568`, `#718096`

## 📱 Responsive Design

The website is fully responsive with breakpoints at:
- **Desktop**: 1200px and up
- **Tablet**: 768px to 1199px
- **Mobile**: 768px and down
- **Small Mobile**: 480px and down

## 🌙 Dark Mode

The website automatically supports dark mode based on user's system preferences. The dark mode styles are defined in `css/responsive.css`.

## 🔧 Browser Support

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## 📧 Contact Form

The contact form includes:
- Form validation
- Service selection dropdown (IT Support, Mobile Development, Software Consulting, IT Automation)
- Success/error notifications
- Simulated form submission (replace with your backend)

To connect to a real backend, update the form submission in `js/main.js`:

```javascript
// Replace the setTimeout with your actual API call
fetch('/api/contact', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify({
        name: name,
        email: email,
        service: service,
        message: message
    })
})
.then(response => response.json())
.then(data => {
    showNotification('Message sent successfully!', 'success');
})
.catch(error => {
    showNotification('Error sending message. Please try again.', 'error');
});
```

## 🚀 Deployment

### GitHub Pages

1. Create a new repository on GitHub
2. Upload your files
3. Go to Settings > Pages
4. Select source branch (usually `main`)
5. Your site will be available at `https://username.github.io/repository-name`

### Netlify

1. Drag and drop your project folder to [Netlify](https://netlify.com)
2. Your site will be deployed instantly
3. You can set up a custom domain in the site settings

### Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts to deploy

### Custom Domain

To use `rcmckain.tech` or `rcmckain.com`:

1. Purchase the domain from a registrar (Namecheap, GoDaddy, etc.)
2. Point the domain to your hosting provider
3. Update the contact email in the HTML file
4. Consider adding SSL certificate for security

## 📈 Performance Tips

1. **Optimize Images**: Use WebP format and compress images
2. **Minify CSS/JS**: Use tools like UglifyJS and CSSNano
3. **Enable Gzip**: Configure your server to compress files
4. **Use CDN**: Serve Font Awesome and Google Fonts from CDN
5. **Lazy Loading**: Images are already set up for lazy loading

## 🛠️ Development

### Adding New Sections

1. Add the HTML structure in `index.html`
2. Add corresponding styles in `css/style.css`
3. Add responsive styles in `css/responsive.css`
4. Add any JavaScript functionality in `js/main.js`

### CSS Organization

- `style.css`: Main styles, layout, and components
- `responsive.css`: Media queries and responsive adjustments

### JavaScript Features

- Navigation with smooth scrolling
- Mobile menu toggle
- Scroll animations and effects
- Contact form validation with service selection
- Loading animations
- Performance optimizations

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to fork this project and customize it for your own portfolio. If you find any bugs or have suggestions, please open an issue.

## 📞 Support

If you need help customizing this portfolio or have questions, feel free to reach out!

---

**Built with ❤️ using HTML, CSS, and JavaScript** 