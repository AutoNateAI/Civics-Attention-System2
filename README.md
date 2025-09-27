# [AdminLTE - Bootstrap 5 Admin Dashboard](https://adminlte.io)

[![npm version](https://img.shields.io/npm/v/admin-lte/latest.svg)](https://www.npmjs.com/package/admin-lte)
[![Packagist](https://img.shields.io/packagist/v/almasaeed2010/adminlte.svg)](https://packagist.org/packages/almasaeed2010/adminlte)
[![cdn version](https://data.jsdelivr.com/v1/package/npm/admin-lte/badge)](https://www.jsdelivr.com/package/npm/admin-lte)
[![Discord Invite](https://img.shields.io/badge/discord-join%20now-green)](https://discord.gg/jfdvjwFqfz)
[![Netlify Status](https://api.netlify.com/api/v1/badges/1277b36b-08f3-43fa-826a-4b4d24614b3c/deploy-status)](https://app.netlify.com/sites/adminlte-v4/deploys)

**AdminLTE** is a fully responsive administration template. Based on **[Bootstrap 5](https://getbootstrap.com/)** framework and also the JavaScript plugins.
Highly customizable and easy to use. Fits many screen resolutions from small mobile devices to large desktops.

## What's New in v4.0.0-rc4

**Latest Release with Enhanced Performance & Updated Dependencies** - Fresh improvements for better development experience:

- **Updated Dependencies** - 8 npm packages updated to latest versions for improved security and performance
- **Refined Mobile Image Loading** - Streamlined path resolution by removing JavaScript runtime fixes
- **Better Performance** - Images now load faster with build-time path generation instead of runtime corrections
- **Latest Tooling** - Updated TypeScript, ESLint, Prettier, Astro, and build tools
- **Zero Runtime Errors** - Eliminated console errors from JavaScript path corrections

**Key Improvements:**
- ✅ All images use relative paths generated at build time
- ✅ No more JavaScript runtime path fixes causing console errors
- ✅ Faster image loading with optimal path resolution
- ✅ Latest development tools and security updates
- ✅ Production-ready with enhanced stability

**Install the latest:**
```bash
npm install admin-lte@4.0.0-rc4
```

See the [CHANGELOG.md](CHANGELOG.md) for complete details.

## Looking for Premium Templates?

AdminLTE.io just opened a new premium templates page. Hand picked to ensure the best quality and the most affordable
prices. Visit <https://adminlte.io/premium> for more information.

!["AdminLTE Presentation"](https://adminlte.io/AdminLTE3.png "AdminLTE Presentation")

**AdminLTE** has been carefully coded with clear comments in all of its JS, SCSS and HTML files.
SCSS has been used to increase code customizability.

## Quick start

### Development

To start developing with AdminLTE:

1. **Install dependencies:** `npm install`
2. **Start development server:** `npm start` *(opens browser at http://localhost:3000)*
3. **Start coding!** Files auto-compile and refresh on changes

### Production Build

To build for production:

1. **Full production build:** `npm run production` *(includes linting and optimization)*
2. **Quick build:** `npm run build` *(faster for development/testing)*

### Available Scripts

- `npm start` - Start development server with file watching
- `npm run build` - Build all assets for development
- `npm run production` - Full production build with linting and bundlewatch
- `npm run lint` - Run all linters (JS, CSS, docs, lockfile)
- `npm run css` - Build CSS only
- `npm run js` - Build JavaScript only
- `npm run docs-compile` - Build documentation site only
- `npm run docs-serve` - Start development server for docs
- `npm run docs-lint` - Lint Astro documentation files
- `npm run docs-format` - Format HTML output

## Deployment

This project includes automated deployment workflows that trigger on pushes to the `main` branch. The deployment system supports multiple platforms:

### GitHub Pages Deployment

1. **Enable GitHub Pages** in your repository settings:
   - Go to Settings → Pages
   - Select "GitHub Actions" as the source

2. **Trigger deployment** by pushing to `main` with the commit message containing `[deploy:github-pages]`:
   ```bash
   git commit -m "Deploy to GitHub Pages [deploy:github-pages]"
   ```

3. **Or deploy manually** using GitHub Actions:
   - Go to Actions tab
   - Select "Deploy to Production" workflow
   - Click "Run workflow"

### Netlify Deployment

1. **Connect your repository** to Netlify:
   - Go to [netlify.com](https://netlify.com)
   - Click "Add new site" → "Import an existing project"
   - Connect your GitHub repository

2. **Configure build settings**:
   - Build command: `npm run docs-compile`
   - Publish directory: `dist`
   - Node version: 18

3. **Add environment variables** (if needed):
   - No special environment variables required for basic deployment

4. **Trigger deployment** by pushing to `main` with the commit message containing `[deploy:netlify]`:
   ```bash
   git commit -m "Deploy to Netlify [deploy:netlify]"
   ```

### Vercel Deployment

1. **Connect your repository** to Vercel:
   - Go to [vercel.com](https://vercel.com)
   - Click "Import Project"
   - Connect your GitHub repository

2. **Configure build settings**:
   - Root Directory: `./`
   - Build Command: `npm run docs-compile`
   - Output Directory: `dist`
   - Install Command: `npm ci`

3. **Add environment variables** (if needed):
   - No special environment variables required for basic deployment

4. **Trigger deployment** by pushing to `main` with the commit message containing `[deploy:vercel]`:
   ```bash
   git commit -m "Deploy to Vercel [deploy:vercel]"
   ```

### Configuration Files

- `netlify.toml` - Netlify deployment configuration
- `vercel.json` - Vercel deployment configuration
- `.github/workflows/deploy.yml` - GitHub Actions deployment workflow

### Deployment Status

You can check deployment status in:
- **GitHub Actions**: Actions tab in your repository
- **Netlify**: Site dashboard on netlify.com
- **Vercel**: Project dashboard on vercel.com
- **GitHub Pages**: Environment deployment URL (shown in Actions)

### Manual Deployment

If you prefer to deploy manually:

```bash
# Build the project
npm run docs-compile

# Deploy to your preferred platform:
# - Upload 'dist' folder to your hosting provider
# - Or use your platform's CLI tools
```

### Troubleshooting

- Ensure Node.js 18+ is installed
- Check that all dependencies are installed: `npm ci`
- Verify build works locally: `npm run docs-compile`
- Check GitHub Actions logs for detailed error information

## Browser Support

AdminLTE supports all modern browsers with the latest Bootstrap 5.3.7:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Platform Support

AdminLTE v4 build scripts work cross-platform:
- **Windows** - Command Prompt, PowerShell, Git Bash
- **macOS** - Terminal, iTerm2
- **Linux** - Bash, Zsh, and other Unix shells

All npm scripts use cross-platform utilities to ensure consistent behavior across different operating systems.

## Sponsorship

Support AdminLTE development by becoming a sponsor or donor.

<p align="center">
  <a href="https://github.com/sponsors/danny007in">
    <img src="https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86" alt="Sponsor on GitHub" />
  </a>
  &nbsp;&nbsp;
  <a href="https://www.paypal.me/daniel007in">
    <img src="https://img.shields.io/static/v1?label=Donate&message=%E2%9D%A4&logo=PayPal&color=%2300457C" alt="Donate via PayPal" />
  </a>
</p>

## Our Sponsors

<p align="center">
  <a href="https://github.com/spizzo14"><img src="https://unavatar.io/github/spizzo14?fallback=https%3A%2F%2Fraw.githubusercontent.com%2FJamesIves%2Fgithub-sponsors-readme-action%2Fdev%2F.github%2Fassets%2Fplaceholder.png" width="50" height="50" alt="User avatar: spizzo14" loading="lazy" /></a>&nbsp;&nbsp;
  <a href="https://github.com/tomhappyblock"><img src="https://unavatar.io/github/tomhappyblock?fallback=https%3A%2F%2Fraw.githubusercontent.com%2FJamesIves%2Fgithub-sponsors-readme-action%2Fdev%2F.github%2Fassets%2Fplaceholder.png" width="50" height="50" alt="User avatar: tomhappyblock" loading="lazy" /></a>&nbsp;&nbsp;
  <a href="https://github.com/stefanmorderca"><img src="https://unavatar.io/github/stefanmorderca?fallback=https%3A%2F%2Fraw.githubusercontent.com%2FJamesIves%2Fgithub-sponsors-readme-action%2Fdev%2F.github%2Fassets%2Fplaceholder.png" width="50" height="50" alt="User avatar: stefanmorderca" loading="lazy" /></a>&nbsp;&nbsp;
  <a href="https://github.com/tito10047"><img src="https://unavatar.io/github/tito10047?fallback=https%3A%2F%2Fraw.githubusercontent.com%2FJamesIves%2Fgithub-sponsors-readme-action%2Fdev%2F.github%2Fassets%2Fplaceholder.png" width="50" height="50" alt="User avatar: tito10047" loading="lazy" /></a>&nbsp;&nbsp;
  <a href="https://github.com/sitchi"><img src="https://unavatar.io/github/sitchi?fallback=https%3A%2F%2Fraw.githubusercontent.com%2FJamesIves%2Fgithub-sponsors-readme-action%2Fdev%2F.github%2Fassets%2Fplaceholder.png" width="50" height="50" alt="User avatar: sitchi" loading="lazy" /></a>&nbsp;&nbsp;
  <a href="https://github.com/npreee"><img src="https://unavatar.io/github/npreee?fallback=https%3A%2F%2Fraw.githubusercontent.com%2FJamesIves%2Fgithub-sponsors-readme-action%2Fdev%2F.github%2Fassets%2Fplaceholder.png" width="50" height="50" alt="User avatar: npreee" loading="lazy" /></a>&nbsp;&nbsp;
  <a href="https://github.com/isaacmorais"><img src="https://unavatar.io/github/isaacmorais?fallback=https%3A%2F%2Fraw.githubusercontent.com%2FJamesIves%2Fgithub-sponsors-readme-action%2Fdev%2F.github%2Fassets%2Fplaceholder.png" width="50" height="50" alt="User avatar: isaacmorais" loading="lazy" /></a>&nbsp;&nbsp;
</p>

<p align="center">
  <a href="https://github.com/sponsors/danny007in">Your avatar here? Become a sponsor</a>
</p>

## Contributing

- Highly welcome.
- For your extra reference check [AdminLTE v4 Contribution Guide](https://github.com/ColorlibHQ/AdminLTE#contributing)
- First thing first, you should have bit knowledge about NodeJS.
- Github Knowledge.
- Install NodeJS LTS version.
- Clone this Repository to your machine and change to `master` branch.
- Go to Cloned Folder.
- In cli/bash run `npm install` it will install dependency from `package.json`.
- After installation completes, run `npm start`
- Cool, Send your changes in PR to `master` branch.


## License

AdminLTE is an open source project by [AdminLTE.io](https://adminlte.io) that is licensed under [MIT](https://opensource.org/licenses/MIT).
AdminLTE.io reserves the right to change the license of future releases.

## Image Credits

- [Pixeden](http://www.pixeden.com/psd-web-elements/flat-responsive-showcase-psd)
- [Graphicsfuel](https://www.graphicsfuel.com/2013/02/13-high-resolution-blur-backgrounds/)
- [Pickaface](https://pickaface.net/)
- [Unsplash](https://unsplash.com/)
- [Uifaces](http://uifaces.com/)
- [Unavatar](https://unavatar.io/)