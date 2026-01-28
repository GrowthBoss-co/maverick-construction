# Favicon Generation Instructions

The website is configured to use favicons, but the actual favicon image files need to be generated from your logo.

## Required Favicon Files

You need to create the following files from `logo.png`:

1. `favicon.ico` - 16x16 and 32x32 sizes combined
2. `favicon-16x16.png` - 16x16 PNG
3. `favicon-32x32.png` - 32x32 PNG
4. `apple-touch-icon.png` - 180x180 PNG (for iOS devices)

## How to Generate Favicons

### Option 1: Online Favicon Generator (Easiest)
1. Go to https://realfavicongenerator.net/
2. Upload your `logo.png` file
3. Customize settings if needed
4. Download the generated favicon package
5. Extract and upload all files to your website root directory

### Option 2: Using Photoshop/GIMP
1. Open `logo.png`
2. Resize to each required size (16x16, 32x32, 180x180)
3. Export as PNG for each size
4. Use an online ICO converter for the .ico file

### Option 3: Using ImageMagick (Command Line)
```bash
# Install ImageMagick first, then:
convert logo.png -resize 16x16 favicon-16x16.png
convert logo.png -resize 32x32 favicon-32x32.png
convert logo.png -resize 180x180 apple-touch-icon.png
convert logo.png -resize 32x32 favicon.ico
```

## After Generation

Once you have the favicon files:
1. Upload them to the root directory of your website
2. Clear browser cache to see the new favicon
3. Test on different devices (desktop, mobile, tablets)

## Current Status

✅ HTML files configured with favicon references
❌ Favicon image files not yet generated (need to be created from logo.png)

The website will work fine without favicons, but browsers will show a default icon instead of your logo.
