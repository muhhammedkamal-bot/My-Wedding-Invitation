# 📋 Wedding Invitation Template - Customization Guide

## Overview
This guide will help you customize the wedding invitation template for your event.

## Step-by-Step Customization

### 1️⃣ Basic Information

Open `template.html` in your text editor and find these sections:

```html
<h1>💕 Couple Name Here 💕</h1>
<h2>Wedding Invitation</h2>
```

**Change to:**
```html
<h1>💕 Your Names Here 💕</h1>
<h2>Your Event Title</h2>
```

### 2️⃣ Event Details

Find the detail items section:
```html
<div class="detail-item">
    <span class="detail-icon">📅</span>
    <span>Date: DD/MM/YYYY</span>
</div>
<div class="detail-item">
    <span class="detail-icon">🕘</span>
    <span>Time: HH:MM</span>
</div>
<div class="detail-item">
    <span class="detail-icon">📍</span>
    <span>Location: City, Country</span>
</div>
```

**Replace with your details:**
```html
<div class="detail-item">
    <span class="detail-icon">📅</span>
    <span>Date: 10/05/2025</span>
</div>
<div class="detail-item">
    <span class="detail-icon">🕘</span>
    <span>Time: 6:00 PM</span>
</div>
<div class="detail-item">
    <span class="detail-icon">📍</span>
    <span>Location: New York, USA</span>
</div>
```

### 3️⃣ Change Colors

**Primary Color:** Find and replace `#ff6b9d` and `#c44569` in the CSS

**Example - Romantic Red Theme:**
```css
/* Replace these colors */
#ff6b9d → #d63384  /* Pink to Red */
#c44569 → #a71930  /* Dark Pink to Dark Red */
```

**Background Gradient:**
```css
background: linear-gradient(135deg, #fff5f7, #ffe8f0, #f0e8ff);
/* Change to your preferred colors */
background: linear-gradient(135deg, #fff0f5, #ffe4f0, #f0f0ff);
```

### 4️⃣ Change Fonts

Find the font-family in CSS:
```css
font-family: 'Arial', sans-serif;
```

**Try these alternatives:**
```css
font-family: 'Georgia', serif;        /* Classic */
font-family: 'Courier New', monospace; /* Modern */
font-family: 'Trebuchet MS', sans-serif; /* Clean */
```

### 5️⃣ Change Gallery Items

Find the gallery section and modify emojis/messages:
```html
<div class="gallery-item" onclick="alert('💐 Beautiful Moments')">💐</div>
<div class="gallery-item" onclick="alert('🎵 Music & Celebration')">🎵</div>
<div class="gallery-item" onclick="alert('🍽️ Delicious Food')">🍽️</div>
<div class="gallery-item" onclick="alert('🎉 Fun & Joy')">🎉</div>
```

**Change to:**
```html
<div class="gallery-item" onclick="alert('🌹 Flowers & Romance')">🌹</div>
<div class="gallery-item" onclick="alert('💍 Rings & Love')">💍</div>
<div class="gallery-item" onclick="alert('🥂 Celebrations')">🥂</div>
<div class="gallery-item" onclick="alert('❤️ Forever')">❤️</div>
```

### 6️⃣ Customize Form Labels

**Confirm Modal:**
```html
<h3>Confirm Your Attendance</h3>
```

**Change to:**
```html
<h3>Will You Join Our Celebration?</h3>
```

**Button Text:**
```html
<button type="submit" class="btn btn-primary" style="width: 100%;">
    Submit Response
</button>
```

### 7️⃣ Adjust Sizes

**Title (h1) Size:**
```css
h1 {
    font-size: 48px;  /* Change this */
}
```

**Smaller screens (mobile):**
```css
@media (max-width: 600px) {
    h1 {
        font-size: 36px;  /* Mobile size */
    }
}
```

### 8️⃣ Add More Details

Add additional information after the main details:
```html
<div class="detail-item">
    <span class="detail-icon">👗</span>
    <span>Dress Code: Formal</span>
</div>
<div class="detail-item">
    <span class="detail-icon">🚗</span>
    <span>Parking: Available</span>
</div>
```

### 9️⃣ Save & Deploy

1. Save your customized file as `index.html`
2. Upload to GitHub
3. Enable GitHub Pages in repository settings
4. Share the link with guests

## 🎨 Color Palette Ideas

### Romantic Wedding
- Primary: `#ff6b9d` (Pink)
- Secondary: `#c44569` (Deep Pink)
- Background: Soft pinks and whites

### Modern Wedding
- Primary: `#2c3e50` (Dark Blue)
- Secondary: `#3498db` (Light Blue)
- Background: Blues and grays

### Classic Wedding
- Primary: `#8b4513` (Brown)
- Secondary: `#daa520` (Gold)
- Background: Creams and golds

### Garden Wedding
- Primary: `#27ae60` (Green)
- Secondary: `#16a085` (Teal)
- Background: Light greens and whites

## 🔧 Common Customizations

### Remove Gallery
Delete this section:
```html
<div class="gallery">
    <!-- All gallery items -->
</div>
```

### Make Buttons Different Colors
```css
.btn-primary {
    background: linear-gradient(135deg, #your-color1, #your-color2);
}

.btn-secondary {
    color: #your-color;
    border-color: #your-color;
}
```

### Change Button Text
```html
<button class="btn btn-primary" onclick="openConfirmModal()">
    🎉 Yes, We're Coming!
</button>
```

### Add Logo/Image
Add this before the couple's names:
```html
<img src="your-image.jpg" style="width: 100px; border-radius: 50%;">
```

## 📱 Testing

1. **Desktop** - Test in Chrome, Firefox, Safari
2. **Mobile** - Test on iPhone and Android
3. **Tablet** - Test on iPad and Android tablets
4. **Forms** - Click buttons and fill forms completely
5. **Console** - Open browser dev tools to check for errors

## 🚀 Deployment Options

### GitHub Pages (Free)
1. Push to GitHub
2. Settings → Pages → Main branch
3. Share the generated link

### Netlify (Free)
1. Connect GitHub repo
2. Deploy automatically
3. Get shareable link

### Vercel (Free)
1. Connect GitHub repo
2. One-click deploy
3. Custom domain available

## 💡 Tips & Tricks

1. **Use Emojis** - Add personality with emojis
2. **Keep Text Short** - Mobile users prefer concise content
3. **Test Links** - Ensure all links work before sharing
4. **Share Early** - Give guests time to respond
5. **Mobile First** - Always test on mobile devices

## ❓ Troubleshooting

### Looks wrong on mobile?
- Check `@media` queries
- Reduce font sizes
- Ensure images are responsive

### Forms not working?
- Check browser console for errors
- Verify form IDs match JavaScript
- Test in different browsers

### Colors look off?
- Clear browser cache
- Check color codes (6 digits after #)
- Test in different browsers

## 🎓 HTML Basics

If you need to add content, use these tags:
```html
<p>Regular text paragraph</p>
<h3>Subheading</h3>
<strong>Bold text</strong>
<em>Italic text</em>
<a href="https://example.com">Link</a>
```

## 📚 Resources

- **Colors:** [Color Picker](https://htmlcolorcodes.com)
- **Emojis:** [Emoji List](https://emojipedia.org)
- **Fonts:** [Google Fonts](https://fonts.google.com)
- **HTML Guide:** [MDN Web Docs](https://developer.mozilla.org)

---

**Happy Customizing!** 💕
Your invitation is ready to share with the world!
