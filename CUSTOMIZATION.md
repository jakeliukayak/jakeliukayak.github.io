# Home Section Customization Guide

This website now supports easy customization of the home section's background and personal images.

## Changing the Background Image

To customize the background image for the home section:

1. Add your background image file to the `images/` folder
2. Edit the `styles.css` file
3. Find the `.hero` section (around line 87)
4. Update the `--hero-background-image` property:

```css
.hero {
    /* Change this line to use your custom background */
    --hero-background-image: url('images/your-background-image.jpg');
    /* ... rest of the styles remain the same ... */
}
```

## Adding Your Personal Photos

To add your personal photos to the right-hand side of the home section:

1. Add your personal images to the `images/` folder
2. Edit the `index.html` file
3. Find the `hero-images` section (around line 36)
4. Replace the placeholder image sources:

```html
<div class="hero-images">
    <img src="images/your-photo-1.jpg" alt="Your description" class="personal-image">
    <img src="images/your-photo-2.jpg" alt="Your description" class="personal-image">
    <img src="images/your-photo-3.jpg" alt="Your description" class="personal-image">
</div>
```

## Tips

- Images work best when they are square (same width and height)
- The personal images are automatically resized to 150x150px on desktop and 120x120px on mobile
- Background images should be high resolution for best quality
- The gradient overlay will still be applied over your background image to maintain text readability