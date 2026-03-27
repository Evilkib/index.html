# Static Website with Vercel Web Analytics

This is a static HTML website configured with Vercel Web Analytics.

## Features

- ✅ Vercel Web Analytics integration
- ✅ Vercel Speed Insights integration
- ✅ Responsive design
- ✅ Modern, clean UI

## Analytics Configuration

This project includes both:

1. **Web Analytics** - Tracks page views, unique visitors, and referrers
2. **Speed Insights** - Monitors site performance metrics

The analytics scripts are integrated directly in the `index.html` file using the static site method recommended by Vercel.

### How It Works

The following scripts are included in the `<head>` section:

```html
<!-- Vercel Web Analytics -->
<script>
    window.va = window.va || function () { (window.vaq = window.vaq || []).push(arguments); };
</script>
<script defer src="/_vercel/insights/script.js"></script>

<!-- Vercel Speed Insights -->
<script>
    window.si = window.si || function () { (window.siq = window.siq || []).push(arguments); };
</script>
<script defer src="/_vercel/speed-insights/script.js"></script>
```

## Deployment

Deploy this project to Vercel:

```bash
vercel deploy
```

Or connect your GitHub repository to Vercel for automatic deployments.

## Viewing Analytics

1. Go to your project dashboard on [Vercel](https://vercel.com)
2. Navigate to the "Analytics" tab
3. View your traffic data (may take a few days of visitor activity to appear)

## Local Development

Simply open `index.html` in your browser, or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (if you have http-server installed)
npx http-server

# Using PHP
php -S localhost:8000
```

## Requirements

- No build tools required
- No npm packages needed
- Pure HTML/CSS/JavaScript
- Deploys directly to Vercel

## Learn More

- [Vercel Web Analytics Documentation](https://vercel.com/docs/analytics/quickstart)
- [Vercel Deployment Documentation](https://vercel.com/docs)
