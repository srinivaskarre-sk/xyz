# Hugo Site with PaperMod Theme

A personal Hugo site using the PaperMod theme, configured for Netlify deployment.

## Local Development

To run the Hugo server locally:

```bash
# Start the development server
hugo server

# Or with drafts enabled
hugo server -D

# The site will be available at http://localhost:1313
```

## Netlify Deployment

This site is configured for automatic deployment on Netlify.

### Netlify Setup

1. Push this repository to GitHub/GitLab/Bitbucket
2. Connect your repository to Netlify
3. Netlify will automatically detect the Hugo configuration
4. The build settings are configured in `netlify.toml`

### Build Configuration

- **Build command**: `hugo --gc --minify`
- **Publish directory**: `public`
- **Hugo version**: latest (automatically uses the most recent Hugo version available on Netlify)

### Updating Base URL

When deploying to Netlify, the `baseURL` in `hugo.toml` will be automatically updated to your Netlify site URL. For production, update the baseURL in `hugo.toml` to match your actual domain.

## Project Structure

- `content/` - Your site content (markdown files)
- `themes/PaperMod/` - The PaperMod theme
- `static/` - Static files (images, etc.)
- `layouts/` - Custom layouts (optional)
- `public/` - Generated static site (git-ignored)

## Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [PaperMod Theme](https://adityatelange.github.io/hugo-PaperMod/)
- [Netlify Hugo Guide](https://docs.netlify.com/integrations/frameworks/hugo/)
