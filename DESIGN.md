---
version: alpha
name: Northfield RENSE Direction
description: Image-first minimalism for small-batch furniture, objects, and studio stories. Original Northfield interpretation informed by RENSE, not a copy of its identity or assets.
colors:
  primary: "#20211E"
  on-primary: "#FAF9F5"
  background: "#F4F2EC"
  surface: "#FAF9F5"
  surface-soft: "#EAE7DE"
  text: "#20211E"
  text-muted: "#67675F"
  accent: "#8B3A2B"
  border: "#C9C7BD"
typography:
  display:
    fontFamily: "Arial, Helvetica Neue, sans-serif"
    fontSize: "56px"
    fontWeight: 500
    lineHeight: 1.02
    letterSpacing: "-1.8px"
  heading:
    fontFamily: "Arial, Helvetica Neue, sans-serif"
    fontSize: "26px"
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "-0.6px"
  body:
    fontFamily: "Arial, Helvetica Neue, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.55
    letterSpacing: "0px"
  label:
    fontFamily: "Arial, Helvetica Neue, sans-serif"
    fontSize: "10px"
    fontWeight: 500
    lineHeight: 1.2
    letterSpacing: "0.12em"
spacing:
  base: "8px"
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "40px"
  xl: "64px"
  section: "80px"
rounded:
  none: "0px"
  sm: "2px"
  md: "2px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "13px 24px"
    height: "44px"
  button-primary-hover:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "12px 23px"
    height: "44px"
  button-secondary-hover:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
  product-image:
    backgroundColor: "{colors.surface-soft}"
    rounded: "{rounded.none}"
  product-card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.text}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "0"
  hairline:
    backgroundColor: "transparent"
    textColor: "{colors.border}"
    height: "1px"
  text-link:
    backgroundColor: "{colors.background}"
    textColor: "{colors.text}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "0"
  metadata:
    backgroundColor: "{colors.background}"
    textColor: "{colors.text-muted}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "0"
---

## Overview

Northfield uses the visual principles of RENSE as a reference direction: minimal furniture and objects, small-batch making, product photography, and a visible path from concept to finished piece. The system is quiet rather than sterile. The product and the making process carry the visual interest.

This is a transformed reference, not a reproduction. RENSE's exact brand assets, copy, code, and photography are not reused.

Reference measured from the public RENSE site and extracted page content. Color values and dimensions below are implementation estimates where browser pixel inspection was unavailable.

## Colors

- **Canvas `#F4F2EC`:** Warm off-white background for a calm gallery-like field.
- **Ink `#20211E`:** Charcoal for headings, navigation, prices, and primary actions.
- **Surface `#FAF9F5`:** Slightly lighter surface used only when grouping a functional area.
- **Surface soft `#EAE7DE`:** Quiet image fallback and supporting surface.
- **Muted `#67675F`:** Secondary copy and product metadata.
- **Border `#C9C7BD`:** Thin structural rules. Borders organize content instead of cards and shadows.
- **Accent `#8B3A2B`:** One restrained oxide accent for active navigation, Heritage, and important state cues.

**Color split rule:** approximately 82% canvas and imagery, 15% ink and text, 3% oxide accent.

**Test:** the accent must not appear as a decorative fill on unrelated sections or repeated badges.

## Typography

Use one neutral sans family for the storefront. The supplied prototype uses an Arial fallback because the reference font is not available. Display type is large, light, and tightly tracked. Body copy stays small, plain, and readable.

- Display: 56px, weight 500, line-height 1.02, tracking -1.8px.
- Heading: 26px, weight 500, line-height 1.15, tracking -0.6px.
- Body: 14px, weight 400, line-height 1.55.
- Label: 10px, weight 500, uppercase, tracking 0.12em.

**Test:** no section heading uses a heavier or more decorative family than the display system.

## Layout

The named pattern is an **image-first editorial storefront**. The Home page uses an asymmetric split hero, a full-width Heritage story, a three-item category rail, and a compact footer. The Shop page gives the product image most of the visual weight. The Studio page uses one featured story followed by an irregular article rail.

- Desktop content width: 1200px maximum.
- Desktop page gutters: 40px.
- Mobile page gutters: 20px.
- Hero image height: approximately 520px desktop, 360px mobile.
- Product image height: approximately 640px desktop, 430px mobile.
- Section spacing: 80px desktop, 54px mobile.
- Product grid gap: 30px.
- Breakpoints: 720px mobile collapse, 1024px desktop composition, 1280px max-width refinement.

**Test:** no desktop section uses a centered text stack with no visual object beside or below it unless it is the intentional Trade form.

## Elevation & Depth

The reference direction avoids floating-card UI. Use no drop shadows on product cards, stories, navigation, or buttons. Use a single 1px hairline to separate real content groups.

**Test:** a product tile must remain structurally clear when all shadows are removed.

## Shapes

The default shape is square. Use 0px radius for image frames, buttons, filters, cards, and inputs. A 2px radius is allowed only for browser-native control tolerance.

**Test:** no pill buttons, circular badges, or soft SaaS cards appear in the storefront.

## Components

### Navigation

A compact wordmark sits left. Four primary destinations sit right: Shop The Collection, Editions, The Studio, and Cart. Trade remains footer-only. The navigation is one line on desktop and becomes horizontally scrollable only where required on small screens.

### Primary button

Use dark ink with off-white text. The button is rectangular, short, and quiet. Hover changes the fill to oxide. Use the same verb for the same action everywhere.

### Product tile

Product tiles are borderless. A large image comes first, followed by a small uppercase category, product name, and muted price. Heritage is an oxide text or state treatment, not a decorative overlay label.

### Product detail

Use a large product image beside concise title, price, stock, purchase action, specifications, and a collapsible Heritage story. The product story is the reason to keep scrolling, not a promotional block.

### Editions

Live, Sold Out, and Archived are real inventory states. Use small text labels and image treatment. Sold-out products retain their identity and sold price without looking like an error state.

### Studio

Use one large featured story and a varied image rail. The first story links directly to the product page. Avoid a generic three-column blog card grid as the only composition.

### Trade

Use a plain editorial page with line sheet, MOQ information, and one enquiry form. No dashboard styling, stats, or portal marketing language.

## Do's and Don'ts

### Do

- Lead with real product or workshop imagery.
- Give the object more area than its metadata.
- Use short, factual copy about making, material, and use.
- Keep one accent color across the entire storefront.
- Use asymmetry sparingly to create visual interest.
- Leave empty space around important objects.
- Keep the Edition archive permanently visible.

### Don't

- Use the supplied Duolingo palette for this furniture brand.
- Use a three-equal-card feature grid as the default section.
- Add shadows, glass, gradients, decorative dots, or fake UI chrome.
- Put Shopify implementation annotations in the customer-facing prototype.
- Use placeholder labels as if they were photography captions.
- Invent precise manufacturing claims or product specifications.
- Clone RENSE's logo, copy, photography, or page code.

## Reference Codification Tests

- **Ratio:** hero media occupies approximately 55% of the hero area. Test: is the visual object at least half of the hero composition?
- **Negative space:** no more than four major content groups appear before the first footer. Test: does every group have a clear job?
- **Accent restraint:** oxide appears only on active states, Heritage, and primary interaction feedback. Test: count unrelated accent fills. It must be zero.
- **Shape:** product images and controls are square or nearly square. Test: search CSS for radius values above 2px.
- **Depth:** no card shadow is needed to understand hierarchy. Test: remove all shadows and inspect the grid.
- **Image priority:** every commerce surface has a real image or an explicitly marked supplied-asset slot. Test: count image-bearing product and story blocks.
- **Copy density:** section subcopy stays below 25 words unless it is the Heritage narrative. Test: flag longer marketing paragraphs for editing.
- **Mobile:** every multi-column section becomes one column below 720px. Test: measure each view at 375px without horizontal overflow.
