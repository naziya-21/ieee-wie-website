# Deployment Guide for IEEE WIE Website

This guide will help you deploy your IEEE WIE website to various platforms. Before proceeding, please make sure you've uploaded all your project files to your GitHub repository.

## Deployment Options

### Option 1: Netlify (Recommended)

Netlify offers a simple deployment process and works well with React applications.

1. **Sign up or log in to [Netlify](https://www.netlify.com/)**
2. **Connect your GitHub repository**
   - Click "New site from Git"
   - Select GitHub as your Git provider
   - Authorize Netlify to access your GitHub account
   - Select your repository (`ieee-wie-website`)

3. **Configure build settings**
   - Build command: `npm run build`
   - Publish directory: `dist`
   - Click "Show advanced" and add the following environment variable:
     - Key: `NODE_VERSION`
     - Value: `16` (or your preferred Node.js version)

4. **Deploy your site**
   - Click "Deploy site"
   - Wait for the build and deployment process to complete

5. **Custom domain (optional)**
   - In Netlify dashboard, go to "Domain settings"
   - Click "Add custom domain" and follow the instructions

### Option 2: Vercel

Vercel is excellent for React applications and offers a great developer experience.

1. **Sign up or log in to [Vercel](https://vercel.com/)**
2. **Import your GitHub repository**
   - Click "Add New..." > "Project"
   - Connect to GitHub and select your repository

3. **Configure project**
   - Framework Preset: Vite
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Install Command: `npm install`

4. **Deploy your site**
   - Click "Deploy"
   - Wait for the build and deployment process to complete

### Option 3: GitHub Pages

For a simpler static site hosting option:

1. **Install gh-pages package locally**
   ```
   npm install --save-dev gh-pages
   ```

2. **Add these scripts to your package.json**
   ```json
   "predeploy": "npm run build",
   "deploy": "gh-pages -d dist"
   ```

3. **Add homepage field to package.json**
   ```json
   "homepage": "https://yourusername.github.io/ieee-wie-website"
   ```

4. **Deploy to GitHub Pages**
   ```
   npm run deploy
   ```

## Troubleshooting Common Deployment Issues

### Build Errors

If you encounter the "could not resolve entry module" error:

1. **Check your vite.config.ts file**
   - Make sure the paths are correct
   - Ensure the root points to the correct directory
   - Verify the build output directory is properly set

2. **Ensure all dependencies are installed**
   ```
   npm install
   ```

3. **Try a clean build**
   ```
   rm -rf node_modules
   npm install
   npm run build
   ```

### Missing Assets or Styles

If your site deploys but is missing styles or assets:

1. **Check your import paths**
   - Make sure all paths use the alias imports (e.g., `@/components/...`)
   - Convert any absolute paths to relative paths

2. **Verify public assets**
   - Ensure any files in the public directory are correctly referenced

## SEO Optimization

To improve your site's visibility:

1. **Update meta tags in index.html**
2. **Add a sitemap.xml file**
3. **Register your site with Google Search Console**

## Performance Optimization

For better performance:

1. **Optimize images before uploading**
2. **Consider adding a CDN for global distribution**
3. **Enable caching headers on your hosting provider**

## Maintenance and Updates

After deployment:

1. **Regularly update dependencies**
2. **Monitor site performance using tools like Google Lighthouse**
3. **Set up analytics to track visitor engagement**

Need further assistance? Feel free to open an issue on the GitHub repository.