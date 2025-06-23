# GridFlow 🌊

> A modern, lightweight, and responsive 12-column CSS Grid system built with mobile-first design principles.

[![CSS Grid](https://img.shields.io/badge/CSS-Grid-blue.svg)](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)
[![Mobile First](https://img.shields.io/badge/Mobile-First-green.svg)](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Responsive/Mobile_first)
[![Responsive](https://img.shields.io/badge/Responsive-Design-orange.svg)](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Responsive_Design)

## ✨ Features

- 🎯 **12-Column Grid System** - Perfect balance of flexibility and simplicity
- 📱 **Mobile-First Approach** - Optimized for mobile devices, scales up beautifully
- 🎨 **CSS Grid Powered** - Modern CSS Grid technology for precise layouts
- 🔧 **Highly Customizable** - Multiple gap sizes, offsets, and utility classes
- 🚀 **Lightweight** - Minimal footprint, maximum performance
- 🌐 **Cross-Browser Compatible** - Works across all modern browsers
- 📐 **Flexible Containers** - Fixed-width and fluid container options

## 📦 Installation

### NPM
```cli
npm install @martyncoup/gridkit
```

### CDN
```html
<link rel="stylesheet" href="path/to/gridflow.css">
```

### Download
Simply download the `gridflow.css` file and include it in your project.

## 🎯 Breakpoints

| Breakpoint | Class Infix | Dimensions |
|------------|-------------|------------|
| Extra small | *none* | <576px |
| Small | `sm` | ≥576px |
| Medium | `md` | ≥768px |
| Large | `lg` | ≥992px |
| Extra large | `xl` | ≥1200px |
| Extra extra large | `xxl` | ≥1400px |

## 🏗️ Basic Structure

```html
<div class="container">
  <div class="row">
    <div class="col-12">
      <!-- Your content here -->
    </div>
  </div>
</div>
```

## 📋 Examples

### 🎯 Basic Grid Layout

```html
<div class="container">
  <div class="row">
    <div class="col-4">Column 1</div>
    <div class="col-4">Column 2</div>
    <div class="col-4">Column 3</div>
  </div>
</div>
```

### 📱 Responsive Grid

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Full width on mobile, half on tablet, third on desktop -->
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <!-- Full width on mobile, half on tablet, third on desktop -->
    </div>
    <div class="col-12 col-md-12 col-lg-4">
      <!-- Full width on mobile and tablet, third on desktop -->
    </div>
  </div>
</div>
```

### 🎨 Grid with Gaps

```html
<div class="container">
  <div class="row gap-lg">
    <div class="col-6">Large gaps</div>
    <div class="col-6">Between columns</div>
  </div>
  
  <div class="row gap-sm">
    <div class="col-3">Small</div>
    <div class="col-3">Gaps</div>
    <div class="col-3">Here</div>
    <div class="col-3">Too</div>
  </div>
</div>
```

### 🔄 Column Offsets

```html
<div class="container">
  <div class="row">
    <div class="col-4 offset-4">
      <!-- Centered 4-column element -->
    </div>
  </div>
  
  <div class="row">
    <div class="col-6 offset-md-3">
      <!-- Offset only on medium screens and up -->
    </div>
  </div>
</div>
```

### 🌊 Fluid Container

```html
<div class="container-fluid">
  <div class="row">
    <div class="col-12">
      <!-- Full width, edge-to-edge -->
    </div>
  </div>
</div>
```

### 🎯 Mixed Column Sizes

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-sm-6 col-md-8">Main content</div>
    <div class="col-12 col-sm-6 col-md-4">Sidebar</div>
  </div>
</div>
```

### 📐 Auto-sizing Columns

```html
<div class="container">
  <div class="row">
    <div class="col-auto">Auto width</div>
    <div class="col">Takes remaining space</div>
    <div class="col-auto">Auto width</div>
  </div>
</div>
```

## 🎛️ Available Classes

### 📊 Containers
- `.container` - Responsive fixed-width container
- `.container-fluid` - Full-width container

### 🏗️ Grid System
- `.row` - Grid row container
- `.col` - Auto-sizing column
- `.col-{1-12}` - Column sizes (1-12)
- `.col-{breakpoint}-{1-12}` - Responsive column sizes

### 📏 Gap Control
- `.gap-sm` - Small gaps (8px)
- `.gap-md` - Medium gaps (16px) - *default*
- `.gap-lg` - Large gaps (24px)
- `.gap-xl` - Extra large gaps (32px)
- `.no-gap` - No gaps

### 🔄 Offsets
- `.offset-{1-11}` - Column offsets
- `.offset-{breakpoint}-{1-11}` - Responsive offsets

### 🎨 Utility Classes
- `.text-left`, `.text-center`, `.text-right` - Text alignment
- `.d-none`, `.d-block`, `.d-flex`, `.d-grid` - Display utilities
- `.d-{breakpoint}-none`, `.d-{breakpoint}-block` - Responsive display

## 🎯 Real-World Examples

### 🏠 Landing Page Layout

```html
<div class="container">
  <!-- Hero Section -->
  <div class="row gap-lg">
    <div class="col-12">
      <h1>Welcome to GridFlow</h1>
    </div>
  </div>
  
  <!-- Features Section -->
  <div class="row gap-md">
    <div class="col-12 col-md-4">
      <h3>🎯 Precise</h3>
      <p>Pixel-perfect layouts every time</p>
    </div>
    <div class="col-12 col-md-4">
      <h3>📱 Responsive</h3>
      <p>Looks great on any device</p>
    </div>
    <div class="col-12 col-md-4">
      <h3>🚀 Fast</h3>
      <p>Lightweight and performance-focused</p>
    </div>
  </div>
</div>
```

### 📝 Blog Layout

```html
<div class="container">
  <div class="row gap-lg">
    <!-- Main Content -->
    <div class="col-12 col-lg-8">
      <article>
        <h2>Blog Post Title</h2>
        <p>Your amazing blog content goes here...</p>
      </article>
    </div>
    
    <!-- Sidebar -->
    <div class="col-12 col-lg-4">
      <aside>
        <h3>Recent Posts</h3>
        <ul>
          <li>Post 1</li>
          <li>Post 2</li>
          <li>Post 3</li>
        </ul>
      </aside>
    </div>
  </div>
</div>
```

### 🛍️ E-commerce Grid

```html
<div class="container">
  <div class="row gap-md">
    <div class="col-6 col-sm-4 col-md-3 col-lg-2">
      <div class="product-card">Product 1</div>
    </div>
    <div class="col-6 col-sm-4 col-md-3 col-lg-2">
      <div class="product-card">Product 2</div>
    </div>
    <div class="col-6 col-sm-4 col-md-3 col-lg-2">
      <div class="product-card">Product 3</div>
    </div>
    <!-- Repeat for more products -->
  </div>
</div>
```

## 🎨 Customization

### 🔧 CSS Custom Properties

You can easily customize GridFlow by overriding CSS custom properties:

```css
:root {
  --gridflow-gap: 20px;
  --gridflow-container-padding: 20px;
  --gridflow-max-width: 1400px;
}
```

### 🎯 Custom Breakpoints

To add custom breakpoints, simply extend the CSS:

```css
/* Custom breakpoint for tablets in portrait mode */
@media (min-width: 600px) {
  .col-tablet-6 { grid-column: span 6; }
  .col-tablet-4 { grid-column: span 4; }
}
```

## 🌟 Browser Support

GridFlow works in all modern browsers that support CSS Grid:

- ✅ Chrome 57+
- ✅ Firefox 52+
- ✅ Safari 10.1+
- ✅ Edge 16+

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. 🍴 Fork the repository
2. 🌿 Create a feature branch
3. 💻 Make your changes
4. ✅ Test thoroughly
5. 📤 Submit a pull request

## 📄 License

GridFlow is released under the MIT License. See LICENSE file for details.

## 🙋‍♀️ FAQ

**Q: How is GridFlow different from Bootstrap?**
A: GridFlow uses modern CSS Grid instead of flexbox, providing more precise control over layouts with cleaner markup.

**Q: Can I use GridFlow with other CSS frameworks?**
A: Absolutely! GridFlow is designed to work alongside other frameworks without conflicts.

**Q: Is GridFlow production-ready?**
A: Yes! GridFlow is thoroughly tested and ready for production use.

**Q: How small is the file size?**
A: The minified CSS file is approximately 15KB, making it lightweight and fast-loading.

---

<div align="center">

Made with ❤️ by developers, for developers

[⭐ Star us on GitHub](https://github.com/martyncoup/gridflow) | [🐛 Report Bug](https://github.com/martyncoup/gridflow/issues) | [💡 Request Feature](https://github.com/martyncoup/gridflow/issues)

</div>