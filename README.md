# PENTECOSTAL GOSPEL CHURCH WEBSITE
## Setup and Image Placement Guide

---

## 📁 FILE STRUCTURE

Your website folder should contain:
```
website-folder/
│
├── index.html          (Main HTML file)
├── styles.css          (CSS styling)
├── script.js           (JavaScript functionality)
│
├── logo.png            (Church logo - YOU NEED TO ADD THIS)
│
├── hero-church.jpg     (Hero section image - YOU NEED TO ADD THIS)
├── about-church.jpg    (About section image - YOU NEED TO ADD THIS)
│
├── ministry-children.jpg   (Children's ministry - YOU NEED TO ADD THIS)
├── ministry-youth.jpg      (Youth ministry - YOU NEED TO ADD THIS)
├── ministry-worship.jpg    (Worship team - YOU NEED TO ADD THIS)
├── ministry-outreach.jpg   (Outreach ministry - YOU NEED TO ADD THIS)
```

---

## 🖼️ IMAGE REQUIREMENTS AND PLACEMENT

### 1. LOGO (logo.png)
- **Location in code**: Lines in `index.html` - navbar and footer
- **Where to place**: In the same folder as index.html
- **Recommended size**: 200x200 pixels (square)
- **Format**: PNG with transparent background (preferred) or JPG
- **What to use**: Your church logo or emblem
- **File name**: Must be exactly `logo.png` (or update the HTML if different)

---

### 2. HERO IMAGE (hero-church.jpg)
- **Location in code**: Line 89 in `styles.css` 
  ```css
  background: linear-gradient(...), url('hero-church.jpg')
  ```
- **Where to place**: Same folder as index.html
- **Recommended size**: 1920x1080 pixels (Full HD)
- **Format**: JPG (for smaller file size)
- **What to use**: 
  - Exterior photo of church building
  - Congregation worshiping (wide shot)
  - Dramatic worship scene
  - Church sanctuary during service
- **File name**: Must be exactly `hero-church.jpg` (or update CSS)

---

### 3. ABOUT IMAGE (about-church.jpg)
- **Location in code**: Line 145 in `index.html`
  ```html
  <img src="about-church.jpg" alt="...">
  ```
- **Where to place**: Same folder as index.html
- **Recommended size**: 800x600 pixels
- **Format**: JPG
- **What to use**:
  - Interior of church sanctuary
  - Pastor preaching
  - Church leaders or members fellowship
  - Church activities/Bible study
- **File name**: Must be exactly `about-church.jpg` (or update HTML)

---

### 4. MINISTRY IMAGES

#### a) Children's Ministry (ministry-children.jpg)
- **Location in code**: Line 254 in `index.html`
- **Recommended size**: 600x400 pixels
- **What to use**: Children in Sunday school, kids activities, youth teaching

#### b) Youth Ministry (ministry-youth.jpg)
- **Location in code**: Line 262 in `index.html`
- **Recommended size**: 600x400 pixels
- **What to use**: Teenagers/young adults gathering, youth worship, activities

#### c) Worship Team (ministry-worship.jpg)
- **Location in code**: Line 270 in `index.html`
- **Recommended size**: 600x400 pixels
- **What to use**: Musicians/singers during worship, choir, instruments

#### d) Outreach Ministry (ministry-outreach.jpg)
- **Location in code**: Line 278 in `index.html`
- **Recommended size**: 600x400 pixels
- **What to use**: Community service, feeding program, evangelism activities

**All ministry images:**
- **Where to place**: Same folder as index.html
- **Format**: JPG
- **File names**: Must match exactly as listed above

---

## 🎨 COLOR SCHEME

The website uses:
- **Primary Color**: Maroon (#800020)
- **Secondary Color**: White (#FFFFFF)
- **Accent**: Light Gray (#f8f8f8)

---

## ✏️ CONTENT TO UPDATE

### In `index.html`, update these sections:

#### 1. SERVICE TIMES (Lines 196-235)
Update with your actual service schedule:
```html
<p class="service-time">Sunday 9:00 AM - 12:00 PM</p>
```

#### 2. CONTACT INFORMATION (Lines 334-362)
Replace placeholder text:
```html
<p>+233 XX XXX XXXX</p>  <!-- Add your phone -->
<p>info@pentecostalgospel.org</p>  <!-- Add your email -->
```

#### 3. SOCIAL MEDIA LINKS (Lines 377-381)
Replace `#` with actual URLs:
```html
<a href="https://facebook.com/yourchurch" class="social-icon">
```

#### 4. EVENTS (Lines 290-328)
Update with your upcoming events:
- Event dates
- Event titles
- Event descriptions
- Times

#### 5. OFFICE HOURS (Lines 363-367)
Update with your actual office hours

---

## 🔧 HOW TO CUSTOMIZE

### Change Church Name:
Find and replace "PENTECOSTAL GOSPEL CHURCH" in `index.html` (appears multiple times)

### Change Location:
Find and replace "Area 50" with your actual location

### Change Colors:
Edit the `:root` section in `styles.css` (lines 11-18):
```css
:root {
    --maroon: #800020;  /* Change this to your color */
    --white: #FFFFFF;
}
```

---

## 📧 EMAIL FORM SETUP

The contact form currently shows an alert. To actually send emails, you need to:

### Option 1: Use EmailJS (Free, Easy)
1. Sign up at [emailjs.com](https://www.emailjs.com/)
2. Get your Service ID and Template ID
3. Uncomment the EmailJS code in `script.js` (lines 127-138)
4. Add EmailJS library to HTML head:
```html
<script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
```

### Option 2: Use Formspree (Free tier available)
1. Sign up at [formspree.io](https://formspree.io/)
2. Update form action in HTML:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 3: Backend Server
Set up PHP, Node.js, or Python backend to handle form submissions

---

## 🚀 LAUNCHING YOUR WEBSITE

### Option 1: Free Hosting
- **Netlify**: Drag and drop your folder
- **Vercel**: Upload via GitHub
- **GitHub Pages**: Free hosting via GitHub
- **Firebase Hosting**: Google's free tier

### Option 2: Web Hosting
- Upload all files to your web host via FTP
- Ensure all files are in the same directory

---

## 📱 MOBILE RESPONSIVE

The website is fully responsive and includes:
- ✅ Mobile navigation menu (hamburger)
- ✅ Touch-friendly buttons
- ✅ Responsive images
- ✅ Mobile-optimized layouts
- ✅ Smooth scrolling

---

## ✅ TESTING CHECKLIST

Before launching:
- [ ] All images are uploaded and displaying correctly
- [ ] Logo appears in navigation and footer
- [ ] Contact phone and email are updated
- [ ] Social media links are working
- [ ] Service times are accurate
- [ ] Mobile menu opens and closes properly
- [ ] All sections scroll smoothly
- [ ] Test on mobile phone and tablet
- [ ] Contact form works (or shows appropriate message)

---

## 🆘 TROUBLESHOOTING

### Images not showing?
1. Check file names match exactly (case-sensitive)
2. Ensure images are in same folder as HTML
3. Check file extensions (.jpg vs .jpeg vs .png)

### Mobile menu not working?
1. Ensure script.js is in same folder
2. Check browser console for JavaScript errors (F12)

### Contact form not working?
1. See "Email Form Setup" section above
2. Default behavior shows alert message

---

## 📞 NEED HELP?

If you need assistance:
1. Check that all files are in the same folder
2. Verify image file names match the code
3. Test in different browsers (Chrome, Firefox, Safari)
4. Clear browser cache (Ctrl + Shift + R)

---

## 🎯 QUICK START

1. ✅ Download all 3 files (index.html, styles.css, script.js)
2. ✅ Put them in one folder
3. ✅ Add your logo.png
4. ✅ Add your church photos (6 images total)
5. ✅ Update contact info in HTML
6. ✅ Open index.html in browser to test
7. ✅ Upload to web host when ready

---

**God bless your ministry! 🙏**

For questions about specific features or customization, feel free to ask!
