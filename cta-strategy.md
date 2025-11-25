# CTA Strategy: PNW Free Mulch Promo Landing Page

**Goal:** Maximize qualified lead generation through strategic call-to-action placement, copy, and tracking

---

## Primary CTA Copy (Consistent Messaging)

### Main CTA Phrase
Use **ONE primary phrase** throughout the page with minimal variations:

**Primary:**
> **Get My Free Mulch Proposal**

**Secondary (same intent, slight variation):**
> **Schedule a Free Mulch Walkthrough**

**Tertiary (for specific contexts):**
> **Request My Free Mulch Proposal**

### Avoid These Weak CTAs
- ❌ "Contact Us"
- ❌ "Learn More"
- ❌ "Get Started"
- ❌ "Submit"
- ❌ "Send"

**Why:** These are generic and don't communicate value or set expectations. "Get My Free Mulch Proposal" is specific, action-oriented, and promises a clear deliverable.

---

## CTA Placement Strategy

### Desktop Layout

#### 1. Hero Section
**Location:** Right side, integrated into form
- **Primary:** Submit button on form ("Get My Free Mulch Proposal")
- **Secondary:** Text link under hero copy ("Schedule a walkthrough" → scrolls to form)

#### 2. Sticky Header
**Location:** Top of page, always visible on scroll
- **Left:** Logo
- **Middle:** Optional navigation (Service Areas, How It Works, FAQ)
- **Right:** **[Get Free Mulch Proposal]** button + phone number (206-202-5161)

**Behavior:**
- Sticky on scroll (appears after user scrolls past hero)
- Button opens form modal or scrolls to form
- Phone number uses CallRail click-to-call tracking

#### 3. End of Each Major Section
Place one CTA button or strong text link at the end of:
- Section 2 (Trust / Who We Serve)
- Section 3 (Why Mulch Matters)
- Section 4 (How It Works)
- Section 5 (Service Areas)
- Section 6 (Proof)

**Format:**
- Button style for primary actions
- Text link for secondary actions
- Both track same conversion event

#### 4. FAQ Section
**Location:** Bottom of FAQ section
**Format:** CTA bar with two actions:
> **Ready to refresh your property's mulch and reduce maintenance headaches?**
> 
> **[Get My Free Mulch Proposal]** • or call **206-202-5161**

---

### Mobile Layout

#### 1. Hero Section
**Location:** Below hero copy, full-width form
- **Primary:** Submit button on form ("Get My Free Mulch Proposal")
- **Secondary:** Phone link ("Call: 206-202-5161")

#### 2. Sticky Bottom Bar
**Location:** Fixed at bottom of viewport, appears after scrolling past hero

**Layout:**
```
┌─────────────────────────────────┐
│  [Call]    [Free Mulch Proposal] │
└─────────────────────────────────┘
```

- **Left:** **Call** (tel: link to 206-202-5161, tracked via CallRail)
- **Right:** **Free Mulch Proposal** (scrolls to form or opens slide-up form)

**Behavior:**
- Always visible after initial scroll
- Dismissible (optional X button in top-right)
- Both actions track conversion events
- High contrast colors for visibility

#### 3. End of Sections
Same as desktop: one CTA per major section

---

## CTA Behavior & Mechanics

### Form Submission CTAs

**Action:** User clicks "Get My Free Mulch Proposal" button

**Behavior:**
1. Form validates required fields
2. On success:
   - Show inline success message: "Thanks! We'll be in touch within 1 business day."
   - OR redirect to thank you page
3. Track conversion events (see Tracking section below)

**Form Fields (all required):**
- Name
- Company / Property Name
- Email
- Phone
- Property Location
- Property Type

**Error Handling:**
- Inline validation messages
- Clear error states
- "Please complete all required fields" message if submit attempted with empty fields

---

### Phone CTAs

**Action:** User clicks phone number (206-202-5161)

**Behavior:**
1. On desktop: Opens phone dialer or CallRail widget
2. On mobile: Initiates phone call directly
3. Track phone click event (see Tracking section)

**Placement:**
- Hero section (secondary CTA)
- Sticky header (desktop)
- Sticky bottom bar (mobile)
- FAQ section (final CTA bar)

**Tracking:**
- CallRail click-to-call tracking
- GA4 event: `phone_click_free_mulch`
- Google Ads conversion (if phone call completed)

---

### Scroll-to-Form CTAs

**Action:** User clicks "Schedule a Free Mulch Walkthrough" or similar text link

**Behavior:**
1. Smooth scroll to form section
2. Optional: Highlight form with subtle animation
3. Track scroll-to-form event

**Alternative:** Open form in modal/overlay
- Faster user experience
- Keeps user on page
- Can be dismissed easily

---

## Tracking & Conversion Events

### Google Analytics 4 (GA4) Events

**Form Submission:**
- Event name: `free_mulch_lead` or `commercial_lead_submit`
- Parameters:
  - `form_location`: "hero" | "section_3" | "section_4" | etc.
  - `property_type`: [value from dropdown]
  - `property_location`: [value from text input]

**Phone Click:**
- Event name: `phone_click_free_mulch`
- Parameters:
  - `phone_location`: "hero" | "header" | "footer" | "mobile_bar"

**CTA Button Click:**
- Event name: `cta_click_free_mulch`
- Parameters:
  - `cta_location`: [section name]
  - `cta_type`: "button" | "text_link"

**Scroll Depth:**
- Event name: `scroll_depth`
- Parameters:
  - `depth`: 25 | 50 | 75 | 100 (percentage)

---

### Google Ads Conversion Tracking

**Primary Conversion:**
- Form submission → `free_mulch_lead`
- Import from GA4 or use native Google Ads conversion tag

**Secondary Conversion:**
- Phone call completion (via CallRail integration)
- Event: `phone_call_completed`

**Conversion Value:**
- Assign estimated value per lead (e.g., $500-1000 per qualified commercial maintenance contract)

---

### CallRail Integration

**Setup:**
- Install CallRail tracking code
- Configure click-to-call numbers
- Set up call tracking for 206-202-5161

**Events to Track:**
- Phone number clicks
- Call duration
- Call recordings (if enabled)
- Call source attribution

**Integration with GA4:**
- Send CallRail events to GA4
- Track phone calls as conversions in Google Ads

---

## Microcopy That Helps Conversion

### Under Main Form
> *No obligation. We only work with commercial properties.*

**Why:** Reduces friction, sets clear qualification criteria

---

### Near CTA Buttons
> *Property managers, facilities teams, and HOAs welcome.*

**Why:** Reinforces target audience, makes users feel included

---

### In "How It Works" Section
> *We'll walk you through the scope and pricing before you decide.*

**Why:** Reduces sales pressure, sets expectation of transparency

---

### Form Success Message
> *Thanks! We'll be in touch within 1 business day.*

**Why:** Sets clear expectation, reduces anxiety about response time

---

### Under Phone Number
> *Call now for immediate assistance*

**Why:** Encourages immediate action for urgent needs

---

## A/B Testing Recommendations

### CTA Copy Variations to Test
1. "Get My Free Mulch Proposal" (baseline)
2. "Schedule a Free Mulch Walkthrough"
3. "Get My Free Mulch Quote"
4. "Request My Free Mulch Proposal"

### CTA Button Color Variations
- Test primary brand color vs. high-contrast color (e.g., orange/red accent)
- Ensure WCAG AA contrast compliance

### Form Placement
- Test form in hero vs. form modal triggered by CTA
- Test form length (6 fields vs. 4 fields)

### Phone CTA Placement
- Test phone number prominence in header vs. footer
- Test click-to-call widget vs. direct tel: link

---

## CTA Performance Metrics to Track

### Primary Metrics
- **Form submission rate:** % of visitors who submit form
- **Phone click rate:** % of visitors who click phone number
- **CTA click-through rate:** % of visitors who click any CTA
- **Conversion rate:** % of visitors who complete form OR call

### Secondary Metrics
- **Time to first CTA click:** How quickly users engage
- **CTA location performance:** Which CTAs perform best
- **Form abandonment rate:** % who start but don't complete form
- **Mobile vs. desktop conversion rates**

### Goals (Benchmarks)
- **Form submission rate:** 2-5% (industry average: 2-3%)
- **Phone click rate:** 1-3%
- **Overall conversion rate:** 3-8% (form + phone)

---

## Implementation Checklist

### Development
- [ ] Implement sticky header with CTA button
- [ ] Implement sticky bottom bar (mobile)
- [ ] Set up form validation and error handling
- [ ] Configure form submission tracking (GA4 + Google Ads)
- [ ] Set up CallRail click-to-call tracking
- [ ] Add smooth scroll behavior for anchor links
- [ ] Test all CTAs on desktop and mobile

### Tracking Setup
- [ ] Install GA4 tracking code
- [ ] Set up conversion events in GA4
- [ ] Configure Google Ads conversion tracking
- [ ] Set up CallRail integration
- [ ] Test event firing in GA4 DebugView
- [ ] Verify conversion tracking in Google Ads

### Content
- [ ] Write all CTA copy variations
- [ ] Add microcopy to reduce friction
- [ ] Create form success/error messages
- [ ] Write thank you page content (if using)

### Testing
- [ ] Test form submission on all devices
- [ ] Test phone click-to-call on mobile
- [ ] Verify all tracking events fire correctly
- [ ] Test form validation and error states
- [ ] Check accessibility (keyboard navigation, screen readers)

---

## Quick Reference: CTA Copy Library

### Primary CTAs
- **Get My Free Mulch Proposal** (use most frequently)
- **Schedule a Free Mulch Walkthrough** (use in context of scheduling)
- **Request My Free Mulch Proposal** (alternative to primary)

### Secondary CTAs
- **Call Now: 206-202-5161** (phone-focused)
- **Schedule a walkthrough** (text link, less prominent)
- **See What We Can Do for Your Property** (proof section)

### Context-Specific CTAs
- **View Service Areas** (Section 2 → scrolls to Section 5)
- **Contact us** (for service area coverage question)
- **See What We Can Do for Your Property** (proof section)

---

*This CTA strategy is designed to maximize conversions while maintaining a professional, non-pushy user experience. All tracking should be implemented before launch to measure performance.*


