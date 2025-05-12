# DirectoryGuide Landing Page Maintenance Guide

This guide will help you maintain and customize the DirectoryGuide landing page. Whether you're new to web development or need a quick reference, follow these detailed instructions for common maintenance tasks.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
The header contains the site logo and navigation menu. To update:

1. **Logo Text**: Find this line and change "DirectoryGuide":
```html
<a href="/" class="text-xl font-bold text-gray-800 hover:text-blue-600 transition-colors duration-300">
    DirectoryGuide
</a>
```

2. **Navigation Links**: Update text in the nav menu:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="mailto:admin@ninja200.online">Contact</a>
</div>
```

### Hero Section
Located at the top of the page. To modify:

1. **Main Heading**: Find and update:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-6">
    How To Start An Online Directory
</h1>
```

2. **Subheading**: Update this text:
```html
<p class="text-xl md:text-2xl text-gray-600 mb-12 leading-relaxed">
    Find A Profitable Directory Niche
</p>
```

### Understanding Tailwind Classes
Common classes used in this page:

- `text-{size}`: Controls text size (xl, 2xl, 4xl, etc.)
- `mb-{size}`: Margin bottom (4, 6, 8, 12, etc.)
- `py-{size}`: Padding top and bottom
- `px-{size}`: Padding left and right
- `bg-{color}-{shade}`: Background colors (blue-600, gray-50, etc.)

Example of modifying a button's appearance:
```html
<!-- Original -->
<a href="https://ninja200.online" class="inline-block bg-blue-600 text-white px-8 py-4 rounded-lg">

<!-- Modified for darker blue and larger padding -->
<a href="https://ninja200.online" class="inline-block bg-blue-700 text-white px-10 py-5 rounded-lg">
```

## Fixing Broken Links

### Current Link Inventory
1. Navigation Menu Links:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="mailto:admin@ninja200.online">Contact</a>
```

2. Call-to-Action Links:
```html
<a href="https://ninja200.online">Start Your Directory Now</a>
```

### Updating Links
To update any link:

1. Locate the `<a>` tag
2. Modify the `href` attribute
3. Test the link

Example:
```html
<!-- Change email address -->
<a href="mailto:admin@ninja200.online">Contact</a>
<!-- Update to -->
<a href="mailto:your.email@domain.com">Contact</a>
```

## Linking Privacy and Terms Pages

### Adding Privacy Policy Link
In the footer section, locate:
```html
<ul class="space-y-2">
    <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
```

Update to:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
```

### Adding Terms of Service Link
Similarly, update:
```html
<li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

To:
```html
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure section IDs match href attributes
   - Check for typos in IDs
   - Verify file paths are correct

2. **Responsive Design Issues**
   - Check Tailwind breakpoint classes (md:, lg:)
   - Test on different screen sizes
   - Verify mobile menu functionality

3. **Style Inconsistencies**
   - Maintain consistent color classes (blue-600, gray-900)
   - Keep consistent spacing (mb-4, py-24)
   - Follow existing padding patterns

### Need Help?
If you encounter issues:
1. Check the HTML structure matches the original
2. Verify all required CSS classes are present
3. Test links in multiple browsers
4. Ensure Alpine.js is properly loaded for FAQ functionality

Remember to always backup your files before making changes, and test thoroughly after each modification.