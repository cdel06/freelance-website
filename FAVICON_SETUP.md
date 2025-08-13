# Favicon Setup for Data Wise Plus Website

## Overview
This website now has favicon support configured with your custom logo. The favicon files are set up but need to be generated from the SVG source.

## Current Setup
- ✅ SVG favicon created: `assets/images/favicon.svg`
- ✅ HTML files updated with favicon links
- ⚠️ PNG and ICO files need to be generated

## Files Created
- `assets/images/favicon.svg` - Your logo in SVG format
- `assets/images/favicon-16x16.png` - Placeholder for 16x16 PNG
- `assets/images/favicon-32x32.png` - Placeholder for 32x32 PNG  
- `assets/images/favicon.ico` - Placeholder for ICO format

## How to Generate the Actual Favicon Files

### Option 1: Online Favicon Generators
1. Go to [favicon.io](https://favicon.io/) or [realfavicongenerator.net](https://realfavicongenerator.net/)
2. Upload your `assets/images/favicon.svg` file
3. Download the generated favicon package
4. Replace the placeholder files with the generated ones

### Option 2: Using Image Editing Software
1. Open `assets/images/favicon.svg` in an image editor (GIMP, Photoshop, etc.)
2. Export as PNG in the following sizes:
   - 16x16 pixels
   - 32x32 pixels
3. Use an online ICO converter to create the favicon.ico file

### Option 3: Command Line (if you have ImageMagick)
```bash
# Convert SVG to PNG files
magick convert assets/images/favicon.svg -resize 16x16 assets/images/favicon-16x16.png
magick convert assets/images/favicon.svg -resize 32x32 assets/images/favicon-32x32.png

# Convert to ICO (combine multiple sizes)
magick convert assets/images/favicon-16x16.png assets/images/favicon-32x32.png assets/images/favicon.ico
```

## HTML Integration
The favicon links have been added to all HTML files:
- `index.html`
- `elements.html` 
- `generic.html`

## Browser Support
- Modern browsers: SVG favicon (best quality)
- Older browsers: ICO format (fallback)
- Mobile devices: PNG formats for different sizes

## Testing
After generating the actual favicon files:
1. Clear your browser cache
2. Refresh the website
3. Check the browser tab to see your favicon
4. Test on different devices and browsers

## Notes
- The SVG favicon provides the best quality and scalability
- ICO format ensures compatibility with older browsers
- PNG formats provide crisp icons for specific sizes
- All favicon files are now properly linked in your HTML
