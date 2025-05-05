# Jacovi E-commerce Website

A multi-page e-commerce website for luxury t-shirts, jackets, accessories, iPhones, and sneakers, built with HTML5, CSS, and JavaScript. Features a sci-fi minimalist design, dark mode, slide-in navigation, product filtering, cart functionality, and contact form validation. Deployed on GitHub Pages.

## Features
- Responsive, mobile-first design.
- Semantic HTML5 with 5+ elements per page.
- Sci-fi minimalist aesthetic with green-neutral colors and dark mode.
- JavaScript interactivity: product filters, cart, form validation, slide-in nav.
- Deployed on GitHub Pages.

## Setup
1. Clone the repository: `git clone https://github.com/username/jacovi-ecommerce.git`
2. Open `index.html` in a browser to view locally.
3. Replace placeholder images in the `images/` folder.

## Deployment
1. Push the repository to GitHub.
2. Go to repository settings, enable GitHub Pages on the `main` branch.
3. Access the live site at `https://username.github.io/jacovi-ecommerce`.

## Dependencies
- [Animate.css](https://animate.style/) for animations.
- [Google Fonts: Orbitron](https://fonts.google.com/specimen/Orbitron) for typography.

## Repository Fix Process - May 2025
### Issue
Files were accidentally committed to the wrong repository (feb-2025-final-project-and-deployment-) instead of the correct repository (jacovi-ecommerce).

### Attempted Solutions
1. Initial Git Commands (Failed Attempts):
```bash
# Attempted to use git commands to move files
git restore --staged feb-2025-final-project-and-deployment-L0RD07K1N9
rm -rf feb-2025-final-project-and-deployment-L0RD07K1N9  # Failed on Windows
rd /s /q feb-2025-final-project-and-deployment-L0RD07K1N9  # PowerShell syntax issues
Remove-Item -Path "feb-2025-final-project-and-deployment-L0RD07K1N9" -Recurse -Force
```

### Successful Resolution
1. Manual File Transfer:
   - Manually copied all website files from wrong repository to correct repository using File Explorer
   - Files moved: HTML files, images, CSS, and JavaScript files

2. Cleaning Up Wrong Repository:
```bash
# In the wrong repository
git rm Hoodie.jpeg about.html accessories.jpg background.jpeg cart.html contact.html iPhone.jpg index.html products.html script.js sneakers.webp style.css t_shirt.jpg
git commit -m "Remove files that were moved to jacovi-ecommerce repository"
git push origin main
```

3. Verification:
   - Confirmed files were successfully deleted from wrong repository
   - Verified files were properly placed in correct repository
   - Both repositories showing clean working trees
   - All changes successfully pushed to GitHub

### Lessons Learned
- Always verify the correct repository before committing changes
- Manual file transfer can be a reliable fallback when git commands face issues
- Important to clean up the source repository after moving files to maintain clean git history