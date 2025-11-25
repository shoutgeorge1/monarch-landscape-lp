# "Why Mulch Matters in the Pacific Northwest" Section Analysis

**Source URL:** https://monarch-new-site-2024.webflow.io/nlscampaign#why-mulch  
**Section ID:** `why-mulch`  
**Analysis Date:** 2025-01-27

---

## 1. TEXT CONTENT

```markdown
## Why Mulch Matters in the Pacific Northwest

### Moisture retention for dry summer months
Keeps soil hydrated, reducing irrigation needs

### Weed suppression and reduced maintenance costs
Naturally inhibits weed growth, saving time and money

### Protection for roots during cold, wet winters
Insulates root systems from harsh PNW weather

### Soil temperature regulation
Maintains consistent soil temperature, promoting healthier plant growth

### Improved landscape appearance and uniformity
Creates a polished, cohesive look for your property

### Prevents erosion in high-rainfall seasons
Protects topsoil from washing away during heavy PNW rains
```

**Note:** The main heading contains an accent span: "**Why Mulch**" (in red/orange) followed by "Matters in the Pacific Northwest" (in black).

---

## 2. TYPOGRAPHY & STYLES

| Element | Font Family | Font Size | Font Weight | Line Height | Text Color (Hex) | Letter Spacing | CSS Class | Usage |
|---------|-------------|-----------|-------------|-------------|------------------|----------------|-----------|-------|
| Main Section Heading (H2) | Inter | 60px | 500 (Medium) | 72px | #000000 | normal | `.heading-94` | Main section title "Why Mulch Matters in the Pacific Northwest" |
| Heading Accent Text (span) | Inter | 60px | 700 (Bold) | 72px | #C8330A | normal | `.text-span-8` | Accent text "Why Mulch" within the H2 heading |
| Feature Subheading (H3) | Inter | 25px | 500 (Medium) | 30px | #000000 | normal | `.heading-95` | Each benefit subheading (e.g., "Moisture retention for dry summer months") |
| Body Paragraph Text (P) | Inter | 16px | 400 (Regular) | 24px | #000000 | normal | `.paragraph-91` | Supporting description text under each subheading |

**Additional Notes:**
- All text uses the **Inter** font family (sans-serif)
- No custom letter spacing applied (all use "normal")
- The accent color `#C8330A` is a red-orange/brick color used for emphasis
- All body text is black (`#000000`)
- Line height ratios: H2 (1.2), H3 (1.2), P (1.5)

---

## 3. IMAGES & ICONS

| # | Type | URL | Alt Text | Dimensions (Natural) | Display Size | Visual Role | CSS Class |
|---|------|-----|----------|---------------------|---------------|-------------|-----------|
| 1 | Icon | `https://marvel-b1-cdn.bc0a.com/f00000000258850/cdn.prod.website-files.com/674e6856ddbe7881b2068ac5/69200a80429e70b79ab70298_nsl%20why%20mulch%20icon1.png` | (empty) | 67 × 67px | 67 × 67px | Small icon for "Moisture retention for dry summer months" | (none) |
| 2 | Icon | `https://marvel-b1-cdn.bc0a.com/f00000000258850/cdn.prod.website-files.com/674e6856ddbe7881b2068ac5/69200c93712ba9593d9dd001_nsl%20why%20mulch%20icon2.png` | (empty) | 67 × 67px | 67 × 67px | Small icon for "Weed suppression and reduced maintenance costs" | (none) |
| 3 | Icon | `https://marvel-b1-cdn.bc0a.com/f00000000258850/cdn.prod.website-files.com/674e6856ddbe7881b2068ac5/69200ca57f6fcd318da74c62_nsl%20why%20mulch%20icon3.png` | (empty) | 67 × 67px | 67 × 67px | Small icon for "Protection for roots during cold, wet winters" | (none) |
| 4 | Icon | `https://marvel-b1-cdn.bc0a.com/f00000000258850/cdn.prod.website-files.com/674e6856ddbe7881b2068ac5/69200cb27b6fb506de05afa2_nsl%20why%20mulch%20icon4.png` | (empty) | 67 × 67px | 67 × 67px | Small icon for "Soil temperature regulation" | (none) |
| 5 | Icon | `https://marvel-b1-cdn.bc0a.com/f00000000258850/cdn.prod.website-files.com/674e6856ddbe7881b2068ac5/69200cc0fb088f4651bf3821_nsl%20why%20mulch%20icon5.png` | (empty) | 67 × 67px | 67 × 67px | Small icon for "Improved landscape appearance and uniformity" | (none) |
| 6 | Icon | `https://marvel-b1-cdn.bc0a.com/f00000000258850/cdn.prod.website-files.com/674e6856ddbe7881b2068ac5/69200cd0fae8f69cef309b87_nsl%20why%20mulch%20icon6.png` | (empty) | 67 × 67px | 67 × 67px | Small icon for "Prevents erosion in high-rainfall seasons" | (none) |
| 7 | Photo | `https://marvel-b1-cdn.bc0a.com/f00000000258850/cdn.prod.website-files.com/674e6856ddbe7881b2068ac5/69200db37b6fb506de05ec20_nsl-hm-image2.jpg` | (empty) | 842 × 802px | 487.5 × 464.3px | Large landscape/mulch photo (appears to be a background or supporting image within the section) | `.image-49` |

**Additional Notes:**
- All 6 icons are square (67×67px) and appear to be custom illustrations
- Icons are positioned alongside their corresponding H3 headings
- The large photo (image-49) is displayed at approximately 58% of its natural size
- **No background images** detected in CSS for this section
- All images lack alt text (accessibility concern)

---

## 4. LAYOUT SUMMARY

### Structure Overview
- **Section Container:** `<section id="why-mulch" class="section-65">`
  - Horizontal padding: `80px` (left and right)
  - Background: Transparent (`rgba(0, 0, 0, 0)`)
  - No borders or rounded corners

### Content Layout
- **Main Container:** Flexbox column layout (`.div-block-171`)
  - Display: `flex`
  - Flex direction: `column` (stacked vertically)
  - Gap between items: `35px`
  - Margin top: `40px`
  - **6 feature items** arranged vertically

### Individual Feature Items
- **Item Structure:** Each item (`.div-block-170`) contains:
  1. Icon image (67×67px) on the left
  2. Text content on the right:
     - H3 subheading
     - Paragraph description
- **Item Width:** `487.5px` per item (desktop)
- **Item Layout:** Flexbox row (icon + text side-by-side)
- **Spacing:** No additional padding or margins on individual items

### Visual Hierarchy
1. **Main heading** (H2) at the top
2. **6 feature blocks** stacked vertically below, each containing:
   - Icon (left)
   - H3 subheading + paragraph (right)
3. **Large photo** (if part of this section) appears after the feature list

### Responsive Behavior
- **Desktop:** Single column layout with items stacked vertically
- **Mobile:** (Not tested, but likely stacks to single column with icon/text potentially reflowing)
- Each feature item maintains a fixed width of `487.5px` on desktop

### Design Elements
- **No borders** or rounded corners on containers
- **No background colors** (transparent section)
- **No gradients** detected
- Clean, minimal design with focus on content hierarchy
- Consistent spacing (35px gap) creates visual rhythm

### Color Scheme
- **Primary text:** Black (`#000000`)
- **Accent color:** Red-orange (`#C8330A`) used for "Why Mulch" text emphasis
- **Background:** Transparent/white

---

## Technical Details

**Section ID:** `why-mulch`  
**Section Class:** `section-65`  
**Container Class:** `div-block-171`  
**Item Class:** `div-block-170`  
**Heading Classes:** `.heading-94` (H2), `.heading-95` (H3)  
**Paragraph Class:** `.paragraph-91`  
**Accent Span Class:** `.text-span-8`

---

*Analysis completed via browser inspection and computed style extraction.*



