# Mobile Testing Checklist — ARCLUME Portfolio

## Before Launch Checklist

### 📱 iPhone Testing
- [ ] iPhone SE (375px)
- [ ] iPhone 12/13 (390px)
- [ ] iPhone 14/15 (393px)
- [ ] iPhone Pro Max (430px)
- [ ] Landscape orientation on all models
- [ ] Notch/Dynamic Island handling (safe areas)

### 🤖 Android Testing
- [ ] Samsung S23/S24 (412px)
- [ ] Google Pixel 7/8 (412px)
- [ ] OnePlus (412px)
- [ ] Motorola (360-412px range)
- [ ] Landscape orientation
- [ ] Notch/Punch hole handling

---

## 🏠 Homepage (index.html)

### Navigation
- [ ] Header sticky on scroll (iOS/Android both)
- [ ] Logo visible and readable
- [ ] Navigation links not wrapping
- [ ] Buttons min 44px × 44px
- [ ] Download CV button clickable

### Hero Section
- [ ] Title fits without overflow
- [ ] Subtitle readable
- [ ] Tags don't wrap awkwardly
- [ ] Buttons stack properly on mobile
- [ ] Showcase carousel visible

### Campaign Slider
- [ ] Slides swipe smoothly
- [ ] Navigation arrows accessible (44px)
- [ ] Dots/indicators clickable
- [ ] Caption text readable
- [ ] No horizontal scroll

### Project Grid
- [ ] 1 column on mobile
- [ ] Images load and display properly
- [ ] Project titles readable
- [ ] Pills/tags don't overlap
- [ ] Hover effects work on touch
- [ ] Click opens lightbox properly

### Lightbox
- [ ] Opens on project click
- [ ] Image scales to fit screen
- [ ] Close button accessible
- [ ] Navigation arrows work (landscape)
- [ ] Swipe to navigate (if enabled)
- [ ] Backdrop dismissal works

### About Section
- [ ] Stats display in 1-2 columns
- [ ] Typography readable
- [ ] Spacing adequate

### Footer
- [ ] QR code visible
- [ ] Contact info readable
- [ ] Social links clickable (44px minimum)

---

## 📄 Case Study Pages (casegenshin.html)

### Sidebar
- [ ] On desktop: sticky sidebar, stays at top on scroll
- [ ] On mobile: sidebar moves below header
- [ ] Links clickable (44px tall)
- [ ] Smooth scrolling to sections

### Main Content
- [ ] Hero image scales properly
- [ ] Title readable
- [ ] Body text doesn't exceed max-width
- [ ] Line height adequate on mobile

### Grids & Tables
- [ ] 2-column → 1-column responsive
- [ ] Tables convert to cards on mobile
- [ ] Table data labels visible
- [ ] KPI tiles responsive

### Gallery
- [ ] 3-col → 2-col → 1-col responsive
- [ ] Images load and display
- [ ] Captions visible
- [ ] No horizontal scroll

### Slider
- [ ] Slides transition smoothly
- [ ] Touch swipe works (if implemented)
- [ ] Navigation buttons accessible
- [ ] Dots/indicators responsive

---

## 🎯 Touch & Interaction Testing

### Button/Link Testing
- [ ] All buttons >= 44px × 44px
- [ ] No accidental taps possible
- [ ] Tap feedback visible
- [ ] Hover states work/don't break mobile

### Form Elements (if any)
- [ ] Input fields min 44px height
- [ ] Enough spacing between inputs
- [ ] Mobile keyboard doesn't hide submit
- [ ] Error messages readable

### Scrolling
- [ ] Smooth scrolling between sections
- [ ] Scroll performance is smooth (FPS)
- [ ] No jank on slow devices
- [ ] Scroll position preserved on back

---

## 🎨 Typography & Readability

### Font Sizes
- [ ] Headings readable at 22px on mobile
- [ ] Body text at least 14px
- [ ] No text smaller than 12px
- [ ] Line height >= 1.5 for body

### Color Contrast
- [ ] Text contrast ratio >= 4.5:1
- [ ] On light colors (if any)
- [ ] On dark backgrounds (current design)
- [ ] Links distinguishable from body text

### Text Overflow
- [ ] No horizontal scroll needed
- [ ] Long words break properly
- [ ] URLs break at hyphens
- [ ] Email addresses readable

---

## 🖼️ Images & Media

### Image Sizing
- [ ] Images fill available width (max 100vw)
- [ ] Aspect ratios maintained
- [ ] No distortion
- [ ] Thumbnail images load fast

### Image Quality
- [ ] Images appear crisp on retina displays (2x, 3x)
- [ ] No pixelation
- [ ] Proper file sizes (optimized)

### Performance
- [ ] No FOUC (Flash of Unstyled Content)
- [ ] Images lazy-loaded (if possible)
- [ ] No layout shift when images load

---

## 🔧 Performance Metrics

### Load Time
- [ ] Initial load under 3s (3G)
- [ ] TTL (Time To Largest Contentful Paint) under 2.5s
- [ ] FCP (First Contentful Paint) under 1.8s

### Runtime Performance
- [ ] No janky animations (60 FPS target)
- [ ] Smooth scrolling
- [ ] Instant response to taps
- [ ] No memory leaks on extended use

### Network
- [ ] Works on 3G (slow networks)
- [ ] Progressive enhancement
- [ ] Assets properly cached

---

## 🌐 Cross-Browser Testing

### Safari (iOS)
- [ ] Viewport settings correct
- [ ] Notch/Dynamic Island spacing
- [ ] Sticky header works
- [ ] Touch interactions smooth
- [ ] No Safari-specific bugs

### Chrome (Android)
- [ ] Color space rendering correct
- [ ] Touch ripple effects work
- [ ] Back gesture works
- [ ] Status bar integration

### Firefox (iOS/Android)
- [ ] Layout identical to Chrome/Safari
- [ ] No flexbox/grid issues
- [ ] CSS grid works properly

---

## ♿ Accessibility Checklist

### Mobile Accessibility
- [ ] Touch targets >= 44px
- [ ] Focus indicators visible (if keyboard used)
- [ ] Color not only means of communication
- [ ] Sufficient contrast ratios
- [ ] Text alternatives for images

### Screen Reader
- [ ] Headings properly structured (h1, h2, h3...)
- [ ] Image alt text present
- [ ] Links have descriptive text (not "click here")
- [ ] Form labels associated with inputs

---

## 🐛 Common Mobile Issues to Check

### Layout Issues
- [ ] No overflow hidden on body causing issues
- [ ] No horizontal scroll
- [ ] Safe area respected (notch/punch hole)
- [ ] No fixed positioning issues

### Interaction Issues
- [ ] Click events fire properly on touch
- [ ] Double-tap zoom doesn't interfere
- [ ] Long-press context menu works
- [ ] Swipe gestures (if any) work smoothly

### Display Issues
- [ ] Z-index layers correct
- [ ] Modal/lightbox doesn't scroll behind
- [ ] Dropdowns/popovers appear above content
- [ ] No element cutoff

---

## 📊 Testing Devices List

**Recommended minimum devices to test:**

1. **iPhone 12** (390px, iOS latest)
2. **iPhone SE** (375px, iOS latest)  
3. **iPhone Pro Max** (430px, iOS latest)
4. **Samsung S23** (412px, Android latest)
5. **Google Pixel 7** (412px, Android latest)
6. **Older Android** (360px, Android 11+)

**Testing Environments:**
- Chrome DevTools (Desktop emulation)
- Safari Developer (macOS)
- Android Studio Emulator
- Real devices (if possible)

---

## 🔍 Quick Test Commands

### Chrome DevTools
1. Press `F12` or `Cmd+Option+I`
2. Click device toggle: `Cmd+Shift+M` (Mac) or `Ctrl+Shift+M` (Windows)
3. Select device from dropdown
4. Test different orientations
5. Check Lighthouse scores (75+ for mobile)

### Testing Checklist Summary
```
✅ Responsive layout (1, 2, 3 columns as appropriate)
✅ Typography readable at all sizes
✅ Touch targets minimum 44px × 44px
✅ No horizontal scrolling
✅ Images scale properly
✅ Interactions smooth and responsive
✅ Performance acceptable (< 3s load)
✅ Accessibility standards met
```

---

## 📈 Success Metrics

- **Responsive**: Looks good on 360px - 430px widths
- **Performant**: Load time under 3s on 3G
- **Accessible**: WCAG 2.1 AA compliance
- **Usable**: All features accessible via touch
- **Touch-friendly**: Min 44px interactive elements

---

## 🚀 Optional Enhancements

- [ ] Add viewport-fit CSS for notch support
- [ ] Implement swipe gestures for carousel
- [ ] Add haptic feedback on interactions
- [ ] Optimize images with WebP format
- [ ] Add service worker for offline support
- [ ] Implement animations only on capable devices

---

**Last Updated**: April 2026
**Portfolio**: ARCLUME — Concept Designer & Pixel Artist
