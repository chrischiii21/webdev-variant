# Consistent Color Scheme - Orange & Blue Theme

## Standard Color Palette

### Primary Colors
```css
--orange: #FF8400          /* Primary accent, CTAs, urgency */
--vista-bleu: #8FA0D8      /* Primary brand color, borders, icons */
--amande: #F9DFC6          /* Light backgrounds, hover states */
--bleu-oxford: #0B0829     /* Dark backgrounds, text */
--pure-white: #FFFFFF      /* Text on dark backgrounds */
```

## Component Background Standards

### Dark Background Components
Use: `bg-gradient-to-br from-[#0B0829] via-[#1a1540] to-[#0B0829]`

**Components:**
- ✅ Navbar
- ✅ CTABanner
- ✅ Statistics
- ✅ WhyChooseUs
- ❌ Footer (needs update)
- ✅ Hero (custom dark gradient)

### Light Background Components
Use: `bg-white` or `bg-[#F9DFC6]`

**Components:**
- FeaturedTemplates
- About sections
- Content areas

## Accent Gradient System

### Orange Accent (Top/Left)
```html
<div class="absolute top-0 left-1/4 w-[600px] h-[600px] -translate-y-1/2 blur-[120px]"
     style="background: radial-gradient(circle, #FF8400 0%, transparent 70%);">
</div>
```

### Vista Bleu Accent (Bottom/Right)
```html
<div class="absolute bottom-0 right-1/4 w-[500px] h-[500px] translate-y-1/2 blur-[100px]"
     style="background: radial-gradient(circle, #8FA0D8 0%, transparent 70%);">
</div>
```

## Grid Pattern Overlay

Standard grid for all dark sections:
```html
<div class="absolute inset-0 opacity-5">
  <div class="absolute inset-0"
       style="background-image: linear-gradient(#8FA0D8 1px, transparent 1px), 
              linear-gradient(90deg, #8FA0D8 1px, transparent 1px); 
              background-size: 50px 50px;">
  </div>
</div>
```

## Border Accents

### Top Border
```html
<div class="absolute top-0 left-0 right-0 h-1 bg-gradient-to-r from-transparent via-[#FF8400] to-transparent">
</div>
```

### Bottom Border
```html
<div class="absolute bottom-0 left-0 right-0 h-1 bg-gradient-to-r from-transparent via-[#8FA0D8] to-transparent">
</div>
```

## Badge Styles

### Orange Badge (Attention/Urgency)
```html
<div class="inline-flex items-center gap-2 bg-gradient-to-r from-[#FF8400] to-[#ff9933] 
            px-4 py-2 rounded-full border border-[#FF8400]/50 
            shadow-[0_0_20px_rgba(255,132,0,0.3)]">
  <div class="w-2 h-2 bg-white rounded-full animate-pulse"></div>
  <span class="text-xs font-bold uppercase tracking-widest text-white">
    BADGE TEXT
  </span>
</div>
```

### Vista Bleu Badge (Information)
```html
<div class="inline-flex items-center gap-2 bg-gradient-to-r from-[#8FA0D8]/20 to-[#8FA0D8]/20 
            px-4 py-2 rounded-full border border-[#8FA0D8]/30">
  <div class="w-2 h-2 bg-[#8FA0D8] rounded-full animate-pulse"></div>
  <span class="text-xs font-bold uppercase tracking-widest text-[#8FA0D8]">
    BADGE TEXT
  </span>
</div>
```

## Heading Styles

### Gradient Heading
```html
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold">
  <span class="bg-gradient-to-r from-white via-[#F9DFC6] to-white bg-clip-text text-transparent">
    Main Text
  </span>
  <span class="text-[#FF8400]"> Accent Word</span>
</h2>
```

### Solid Heading
```html
<h2 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white">
  Heading Text
</h2>
```

## Card Styles

### Dark Glassmorphism Card
```html
<div class="bg-gradient-to-br from-[#0B0829]/80 to-[#1a1540]/80 
            border-2 border-[#8FA0D8]/30 
            hover:border-[#FF8400]/60 
            hover:shadow-[0_0_30px_rgba(255,132,0,0.3)]
            rounded-3xl p-6 backdrop-blur-sm 
            transition-all duration-500">
  <!-- Card content -->
</div>
```

### Light Card
```html
<div class="bg-white border-2 border-[#8FA0D8]/20 
            hover:border-[#FF8400]/40 
            rounded-3xl p-6 
            shadow-lg hover:shadow-xl 
            transition-all duration-500">
  <!-- Card content -->
</div>
```

## Icon Backgrounds

### Gradient Icon Background
```html
<div class="w-14 h-14 rounded-2xl 
            bg-gradient-to-br from-[#FF8400]/30 to-[#8FA0D8]/30 
            border border-[#8FA0D8]/20 
            flex items-center justify-center 
            group-hover:rotate-12 group-hover:scale-110 
            transition-transform duration-500">
  <!-- Icon SVG -->
</div>
```

## Button Styles

### On Dark Backgrounds (theme="dark")
- Primary: Vista Bleu → Amande hover
- Secondary: Orange → Amande hover
- Outline: Vista Bleu border → Amande hover

### On Light Backgrounds (theme="light")
- Primary: Vista Bleu → Bleu Oxford hover
- Secondary: Orange → Bleu Oxford hover
- Outline: Vista Bleu border → Bleu Oxford hover

## Text Colors

### On Dark Backgrounds
- Primary text: `text-white` or gradient
- Secondary text: `text-[#F9DFC6]/90`
- Accent text: `text-[#FF8400]`
- Muted text: `text-gray-300`

### On Light Backgrounds
- Primary text: `text-[#0B0829]`
- Secondary text: `text-gray-600`
- Accent text: `text-[#FF8400]`
- Muted text: `text-gray-500`

## Hover Effects

### Card Hover
```css
hover:border-[#FF8400]/60
hover:shadow-[0_0_30px_rgba(255,132,0,0.3)]
hover:-translate-y-2
```

### Icon Hover
```css
group-hover:rotate-12
group-hover:scale-110
transition-transform duration-500
```

### Link Hover
```css
hover:text-[#FF8400]
transition-colors duration-200
```

## Shadow System

### Default Shadow
```css
shadow-[0_4px_20px_rgba(143,160,216,0.2)]
```

### Hover Shadow (Orange)
```css
hover:shadow-[0_12px_40px_rgba(255,132,0,0.4)]
```

### Hover Shadow (Vista Bleu)
```css
hover:shadow-[0_12px_40px_rgba(143,160,216,0.3)]
```

### Glow Shadow (Orange)
```css
shadow-[0_0_20px_rgba(255,132,0,0.3)]
```

### Glow Shadow (Vista Bleu)
```css
shadow-[0_0_20px_rgba(143,160,216,0.3)]
```

## Animation Standards

### Floating Orbs
```css
@keyframes float {
  0%, 100% { transform: translateY(0) scale(1); }
  50% { transform: translateY(-20px) scale(1.05); }
}
.animate-float {
  animation: float 8s ease-in-out infinite;
}
```

### Pulse
```css
animate-pulse /* Built-in Tailwind */
```

### Fade In Up
```css
@keyframes fade-in-up {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
```

## Component Checklist

### ✅ Properly Styled (Dark Theme)
- Navbar
- CTABanner
- Statistics
- WhyChooseUs
- Hero (custom)

### ❌ Needs Update
- Footer (missing dark background)

### 🔍 Needs Review
- FeaturedTemplates (should be light)
- About sections (should be light)
- Content pages

## Implementation Priority

1. **High Priority**: Footer - add dark background to match other sections
2. **Medium Priority**: Review all page sections for consistency
3. **Low Priority**: Fine-tune hover states and animations

## Quick Reference

**Dark Section Template:**
```html
<section class="relative text-white py-20 overflow-hidden 
                bg-gradient-to-br from-[#0B0829] via-[#1a1540] to-[#0B0829]">
  <!-- Orange accent gradient -->
  <!-- Vista Bleu accent gradient -->
  <!-- Grid pattern -->
  <!-- Top border (Orange) -->
  <!-- Bottom border (Vista Bleu) -->
  <!-- Content -->
</section>
```

**Light Section Template:**
```html
<section class="relative py-20 overflow-hidden bg-white">
  <!-- Subtle accents -->
  <!-- Content -->
</section>
```

This ensures every component follows the same visual language and creates a cohesive, professional website experience!
