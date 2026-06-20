# Kanak's Portfolio

A modern, responsive portfolio website showcasing cybersecurity experience, projects, and skills.

## Features

- 🎨 Clean, professional design with cybersecurity theme
- 📱 Fully responsive layout
- ⚡ Vercel Speed Insights for performance monitoring
- 🔒 Security-focused project showcase
- 📧 Contact form integration with Formspree

## Vercel Speed Insights

This portfolio includes **Vercel Speed Insights** to monitor real-world performance metrics and Core Web Vitals.

### What is Speed Insights?

Vercel Speed Insights automatically tracks:
- **Core Web Vitals** (LCP, FID, CLS)
- **Time to First Byte (TTFB)**
- **First Contentful Paint (FCP)**
- Real user performance data

### Implementation

Speed Insights is integrated using the CDN approach for static HTML sites:

```html
<script type="module">
  import { injectSpeedInsights } from 'https://cdn.jsdelivr.net/npm/@vercel/speed-insights@1/dist/index.js';
  injectSpeedInsights();
</script>
```

The script is loaded at the end of the page (before `</body>`) using ES modules, ensuring:
- ✅ Non-blocking page load
- ✅ Automatic performance tracking
- ✅ No build step required
- ✅ Works with static hosting

### Viewing Insights

Once deployed on Vercel:

1. Enable Speed Insights in your Vercel project dashboard
2. Navigate to the **Speed Insights** tab
3. View real-time performance metrics and Core Web Vitals
4. Data appears after users visit your site

> **Note**: Speed Insights does not track data in development mode. Performance metrics are only collected in production deployments.

## Development

To run locally:

```bash
# Using Python's built-in HTTP server
python3 -m http.server 8000

# Or using Node.js
npx serve
```

Then open `http://localhost:8000` in your browser.

## Deployment

This site is optimized for deployment on **Vercel**:

1. Connect your GitHub repository to Vercel
2. Vercel will automatically detect this as a static site
3. Enable Speed Insights in project settings
4. Deploy!

## Technologies

- **HTML5** & **CSS3** (vanilla, no frameworks)
- **JavaScript** (ES6+, no dependencies)
- **Vercel Speed Insights** for performance monitoring
- **Formspree** for contact form handling
- **Google Fonts** (Space Grotesk, Inter, JetBrains Mono)

## License

MIT License - feel free to use this as inspiration for your own portfolio!

---

**Designed & built by Kanak** · Delhi, India · 2026
