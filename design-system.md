# SENECA — Design System Specification

---

## 1. COLOR PALETTE

### Primary Colors

| Name | HEX | RGB | Usage |
|------|-----|-----|-------|
| **Anchor Black** | `#1A1A1A` | 26, 26, 26 | Primary headings, navigation, logo, authority text |
| **Graphite** | `#2D2D2D` | 45, 45, 45 | Secondary headings, emphasis text |
| **Body Gray** | `#4A4A4A` | 74, 74, 74 | Body text, paragraphs, descriptions |
| **Soft Gray** | `#6B6B6B` | 107, 107, 107 | Secondary body text, captions, metadata |

### Background Colors

| Name | HEX | RGB | Usage |
|------|-----|-----|-------|
| **Pure White** | `#FFFFFF` | 255, 255, 255 | Primary background, content areas |
| **Off White** | `#FAFAFA` | 250, 250, 250 | Alternate section backgrounds |
| **Light Gray** | `#F5F5F5` | 245, 245, 245 | Cards, containers, subtle separation |
| **Warm White** | `#F8F7F5` | 248, 247, 245 | Optional warm alternative for sections |

### Accent Colors

| Name | HEX | RGB | Usage |
|------|-----|-----|-------|
| **Performance Green** | `#2E7D5A` | 46, 125, 90 | Positive metrics only, growth indicators, key highlights |
| **Steel Blue** | `#5A6C7D` | 90, 108, 125 | Links, dividers, secondary accents |
| **Muted Gold** | `#8B7355` | 139, 115, 85 | Optional premium accent, sparingly used |

### Utility Colors

| Name | HEX | RGB | Usage |
|------|-----|-----|-------|
| **Border Light** | `#E5E5E5` | 229, 229, 229 | Card borders, dividers, separators |
| **Border Medium** | `#D0D0D0` | 208, 208, 208 | Active borders, form fields |
| **Disabled** | `#B0B0B0` | 176, 176, 176 | Disabled states, inactive elements |

### Color Usage Rules

1. **Accent colors must not exceed 10% of total UI surface**
2. **Performance Green** is reserved exclusively for:
   - Positive percentage changes
   - Growth metrics
   - Success states
   - Key call-to-action buttons (primary only)
3. **Never use**:
   - Bright gradients
   - Neon colors
   - High-saturation accents
   - Multiple accent colors in the same section
4. **Backgrounds** should be predominantly white or off-white
5. **Text on dark backgrounds**: Use `#FFFFFF` or `#F5F5F5`

---

## 2. TYPOGRAPHY SYSTEM

### Primary Typeface
**Montserrat** — Google Fonts

Fallback stack: `'Montserrat', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`

### Type Scale

| Element | Size (Desktop) | Size (Mobile) | Weight | Line Height | Letter Spacing |
|---------|---------------|---------------|--------|-------------|----------------|
| **H1** | 48px / 3rem | 36px / 2.25rem | 600 (Semi-Bold) | 1.2 | -0.02em |
| **H2** | 36px / 2.25rem | 28px / 1.75rem | 600 (Semi-Bold) | 1.25 | -0.01em |
| **H3** | 28px / 1.75rem | 22px / 1.375rem | 600 (Semi-Bold) | 1.3 | 0 |
| **H4** | 22px / 1.375rem | 18px / 1.125rem | 500 (Medium) | 1.35 | 0 |
| **H5** | 18px / 1.125rem | 16px / 1rem | 500 (Medium) | 1.4 | 0 |
| **Body Large** | 18px / 1.125rem | 16px / 1rem | 400 (Regular) | 1.7 | 0.01em |
| **Body** | 16px / 1rem | 15px / 0.9375rem | 400 (Regular) | 1.7 | 0.01em |
| **Body Small** | 14px / 0.875rem | 13px / 0.8125rem | 400 (Regular) | 1.6 | 0.01em |
| **Caption** | 12px / 0.75rem | 12px / 0.75rem | 400 (Regular) | 1.5 | 0.02em |
| **Overline** | 12px / 0.75rem | 11px / 0.6875rem | 500 (Medium) | 1.4 | 0.1em |

### Metric & Number Typography

| Element | Size | Weight | Notes |
|---------|------|--------|-------|
| **Large Metric** | 42px / 2.625rem | 600 | Hero statistics, key figures |
| **Medium Metric** | 28px / 1.75rem | 600 | Card statistics |
| **Small Metric** | 20px / 1.25rem | 500 | Inline metrics |
| **Percentage** | Inherit | 500 | Use tabular figures |

### Typography Rules

1. **Never use weights above 600** (Semi-Bold)
2. **Avoid ultra-light weights** (100-200) for body text
3. **Line height for body text**: Minimum 1.6, preferred 1.7
4. **Maximum line width**: 70-75 characters for optimal readability
5. **Headings**: Allow natural word breaks, avoid orphans
6. **Numbers**: Use `font-variant-numeric: tabular-nums` for aligned data
7. **All caps**: Use sparingly, only for labels and overlines

---

## 3. SPACING SYSTEM

### Base Unit
**8px** — All spacing derived from multiples of 8

### Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `space-1` | 4px | Tight spacing, icon gaps |
| `space-2` | 8px | Inline elements, small gaps |
| `space-3` | 16px | Related element groups |
| `space-4` | 24px | Component internal padding |
| `space-5` | 32px | Section internal spacing |
| `space-6` | 48px | Between components |
| `space-7` | 64px | Section separators (mobile) |
| `space-8` | 96px | Section separators (desktop) |
| `space-9` | 128px | Major section breaks |
| `space-10` | 160px | Hero/footer spacing |

### Section Padding

| Section Type | Desktop | Tablet | Mobile |
|--------------|---------|--------|--------|
| **Hero** | 160px top, 128px bottom | 120px top, 96px bottom | 80px top, 64px bottom |
| **Standard Section** | 96px vertical | 72px vertical | 56px vertical |
| **Compact Section** | 64px vertical | 48px vertical | 40px vertical |
| **Footer** | 80px top, 48px bottom | 64px top, 40px bottom | 48px top, 32px bottom |

### Container Widths

| Container | Max Width | Padding (Desktop) | Padding (Mobile) |
|-----------|-----------|-------------------|------------------|
| **Full** | 1440px | 80px horizontal | 24px horizontal |
| **Content** | 1200px | 80px horizontal | 24px horizontal |
| **Narrow** | 800px | 80px horizontal | 24px horizontal |
| **Text** | 680px | 40px horizontal | 24px horizontal |

### Component Spacing

| Component | Internal Padding | Gap Between |
|-----------|-----------------|-------------|
| **Card** | 32px | 24px |
| **Button** | 16px vertical, 32px horizontal | 16px |
| **Form Field** | 16px | 24px |
| **List Item** | 16px vertical | 0 |
| **Navigation Item** | 12px vertical, 24px horizontal | 8px |

---

## 4. UI ELEMENTS

### Buttons

**Primary Button**
- Background: `#1A1A1A` (Anchor Black)
- Text: `#FFFFFF`
- Padding: 16px 32px
- Border-radius: 4px
- Font: 14px, Medium (500), uppercase, 0.05em letter-spacing
- Hover: Background `#2D2D2D`
- Transition: 200ms ease

**Secondary Button**
- Background: transparent
- Border: 1px solid `#1A1A1A`
- Text: `#1A1A1A`
- Padding: 16px 32px
- Border-radius: 4px
- Hover: Background `#F5F5F5`

**Accent Button** (Use sparingly)
- Background: `#2E7D5A` (Performance Green)
- Text: `#FFFFFF`
- Same dimensions as Primary
- Reserved for primary CTA only

**Button Rules**
- No pill-shaped buttons (max border-radius: 6px)
- No shadows on buttons
- No gradient backgrounds
- Minimum touch target: 44px height

### Cards

**Standard Card**
- Background: `#FFFFFF`
- Border: 1px solid `#E5E5E5`
- Border-radius: 8px
- Padding: 32px
- Shadow: None (or very subtle: `0 1px 3px rgba(0,0,0,0.04)`)
- Hover: Border `#D0D0D0`, subtle lift optional

**Feature Card**
- Background: `#F5F5F5`
- Border: None
- Border-radius: 8px
- Padding: 40px

### Form Elements

**Input Fields**
- Height: 52px
- Border: 1px solid `#D0D0D0`
- Border-radius: 4px
- Padding: 16px
- Focus: Border `#1A1A1A`
- Font: 16px Regular

**Labels**
- Font: 14px Medium
- Color: `#4A4A4A`
- Margin-bottom: 8px

### Dividers

**Horizontal Rule**
- Height: 1px
- Color: `#E5E5E5`
- Margin: 48px 0

**Section Divider**
- Height: 1px
- Color: `#E5E5E5`
- Max-width: 120px
- Centered

---

## 5. IMAGERY GUIDELINES

### Photography Style

**Preferred Subjects:**
- Architecture and interiors
- Cityscapes and landmarks (Uzbekistan)
- Landscape and natural environments
- Texture and material details
- Construction progress (documentary style)

**Avoid:**
- Stock photo cliches (handshakes, pointing at screens)
- Overly posed people
- Heavy filters or color grading
- Busy or cluttered compositions

### Image Treatment

- **Resolution**: Minimum 2x for retina displays
- **Aspect ratios**: 16:9 (hero), 4:3 (cards), 1:1 (thumbnails)
- **Color**: Natural, minimal post-processing
- **Overlay**: If text over image, use subtle gradient overlay (black 0% to 60% opacity)

### Image Rules

1. No permanent blur effects
2. No heavy vignettes
3. No saturated color filters
4. Prefer natural daylight photography
5. Maintain consistent visual temperature across site

---

## 6. MOTION & ANIMATION

### Principles

- Motion is subtle and purposeful
- No bouncy or playful effects
- No attention-grabbing animations
- Enhance usability, not decoration

### Timing

| Type | Duration | Easing |
|------|----------|--------|
| **Micro-interaction** | 150ms | ease-out |
| **Standard transition** | 200ms | ease |
| **Page transition** | 300ms | ease-in-out |
| **Reveal animation** | 400-600ms | ease-out |

### Allowed Animations

- Fade in on scroll (opacity 0 to 1)
- Subtle slide up (transform: translateY(20px) to 0)
- Button hover state changes
- Card hover elevation
- Menu open/close

### Prohibited Animations

- Parallax scrolling
- Bouncing elements
- Rotating or spinning
- Complex sequenced animations
- Auto-playing carousels
- Pulsing or glowing effects

---

## 7. UI TONE SUMMARY

SENECA's visual system embodies quiet authority and institutional credibility. The design language is intentionally restrained — favoring generous white space, disciplined typography, and a muted color palette over visual excitement. Every element serves a functional purpose; there is no decoration for its own sake. The overall impression should feel like reading a well-structured investment memo: clear, professional, and trustworthy. This is design that recedes, allowing content and data to command attention while the interface provides calm, confident support.

---

## 8. ELEMENTOR IMPLEMENTATION NOTES

### Global Settings

**Colors (Add to Elementor Global Colors):**
- Primary: `#1A1A1A`
- Secondary: `#4A4A4A`
- Text: `#4A4A4A`
- Accent: `#2E7D5A`
- Background: `#FFFFFF`
- Background Alt: `#F5F5F5`

**Typography (Add to Elementor Global Fonts):**
- Primary: Montserrat
- Secondary: Montserrat
- Text: Montserrat
- Accent: Montserrat

### Section Settings

- Default padding: 96px top/bottom (desktop), 56px (mobile)
- Content width: 1200px
- Column gap: 24px
- Widget gap: 24px

### Recommended Widgets

- Heading (not animated heading)
- Text Editor
- Image
- Divider (styled minimal)
- Spacer
- Icon List
- Button

### Widgets to Avoid

- Animated Headline
- Price Table
- Countdown
- Testimonial Carousel
- Image Carousel (unless manual control)
- Progress Bar
- Any widget with default animations

### CSS Variables (Add to Custom CSS)

```css
:root {
  --seneca-black: #1A1A1A;
  --seneca-graphite: #2D2D2D;
  --seneca-body: #4A4A4A;
  --seneca-soft: #6B6B6B;
  --seneca-white: #FFFFFF;
  --seneca-off-white: #FAFAFA;
  --seneca-light: #F5F5F5;
  --seneca-green: #2E7D5A;
  --seneca-steel: #5A6C7D;
  --seneca-border: #E5E5E5;

  --seneca-space-sm: 8px;
  --seneca-space-md: 24px;
  --seneca-space-lg: 48px;
  --seneca-space-xl: 96px;

  --seneca-radius: 4px;
  --seneca-radius-lg: 8px;

  --seneca-transition: 200ms ease;
}

body {
  font-family: 'Montserrat', -apple-system, BlinkMacSystemFont, sans-serif;
  font-size: 16px;
  line-height: 1.7;
  color: var(--seneca-body);
  -webkit-font-smoothing: antialiased;
}

h1, h2, h3, h4, h5, h6 {
  color: var(--seneca-black);
  font-weight: 600;
}
```

---

*Document Version: 1.0*
*Prepared for: seneca.uz*
*Framework: Elementor (WordPress)*
