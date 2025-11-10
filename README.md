# KCNails Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain, customize, and update your KCNails landing page. Whether you're new to web development or looking for a refresher, we've broken everything down into clear, step-by-step instructions.

---

## Table of Contents

1. [Overview of the Landing Page](#overview-of-the-landing-page)
2. [Updating Text Content](#updating-text-content)
3. [Customizing Styles with Tailwind CSS](#customizing-styles-with-tailwind-css)
4. [Fixing and Managing Links](#fixing-and-managing-links)
5. [Creating and Linking Policy Pages](#creating-and-linking-policy-pages)
6. [Troubleshooting Common Issues](#troubleshooting-common-issues)
7. [Best Practices for Maintenance](#best-practices-for-maintenance)

---

## Overview of the Landing Page

Your KCNails landing page is built with:

- **HTML5**: The structure and content
- **Tailwind CSS**: A utility-first CSS framework for styling (loaded from CDN)
- **Font Awesome Icons**: Beautiful icons for visual elements
- **Vanilla JavaScript**: Interactive features like mobile menu and FAQ accordion

### Main Sections of the Page

| Section | Purpose | Location in Code |
|---------|---------|------------------|
| Header Navigation | Logo, menu links, "Shop Now" button | Lines 15-52 |
| Hero Section | Main headline, call-to-action, stats | Lines 54-106 |
| Features Section | Three feature cards (Vegan, Chip-Resistant, Shipping) | Lines 108-220 |
| Benefits Section | Three benefit cards with icons | Lines 222-350 |
| Testimonials | Customer reviews in grid layout | Lines 352-530 |
| About Us | Brand story and stats | Lines 532-575 |
| FAQ Section | Expandable questions and answers | Lines 577-730 |
| CTA Section | Final call-to-action with background image | Lines 732-765 |
| Footer | Links, contact info, social media | Lines 767-880 |

---

## Updating Text Content

### Understanding the HTML Structure

Before making changes, it's important to understand what you're looking at. HTML uses **tags** to organize content:

```html
<h1>This is a heading</h1>
<p>This is a paragraph of text</p>
<a href="https://example.com">This is a link</a>
```

The text between the opening tag (`<h1>`) and closing tag (`</h1>`) is what appears on your page.

### How to Update Text: Step-by-Step

**Step 1: Open your HTML file**
- Locate your `index.html` file on your computer
- Right-click and select "Open with" → choose a text editor (Notepad, VS Code, Sublime Text, etc.)

**Step 2: Find the text you want to change**
- Use `Ctrl+F` (Windows) or `Cmd+F` (Mac) to open the Find function
- Search for the text you want to change

**Step 3: Edit the text**
- Replace the old text with your new text
- Keep the HTML tags (`<h1>`, `</h1>`, etc.) exactly as they are

**Step 4: Save your file**
- Press `Ctrl+S` (Windows) or `Cmd+S` (Mac)
- Refresh your browser to see the changes

---

### Key Text Sections to Update

#### 1. **Page Title** (What appears in the browser tab)

**Location**: Line 7
**Current Code**:
```html
<title>Empower Your Style: KCNails UKR - Professional Nail Products</title>
```

**How to Update**:
1. Find this line using Ctrl+F
2. Replace the text between `<title>` and `</title>` with your new title
3. **Example**:
   ```html
   <title>Your New Title Here - KCNails</title>
   ```

**Why This Matters**: This is what appears in the browser tab and search engine results.

---

#### 2. **Meta Description** (What shows in Google search results)

**Location**: Line 6
**Current Code**:
```html
<meta name="description" content="Discover beautiful, professional-grade nail products from KCNails UKR. Vegan, cruelty-free formulas with salon-quality finish.">
```

**How to Update**:
1. Find this line using Ctrl+F
2. Replace the text in the `content=""` section
3. Keep it between 150-160 characters for best results
4. **Example**:
   ```html
   <meta name="description" content="Your new description here - keep it concise and informative.">
   ```

---

#### 3. **Main Headline (Hero Section)**

**Location**: Lines 72-75
**Current Code**:
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold mb-6 leading-tight">
    <span class="block mb-2">Empower Your</span>
    <span class="gradient-text">Style</span>
</h1>
```

**How to Update**:
1. Find "Empower Your" using Ctrl+F
2. Replace "Empower Your" with your new first line
3. Replace "Style" with your new second line (this one has special gradient styling)
4. **Example**:
   ```html
   <h1 class="text-5xl md:text-6xl lg:text-7xl font-bold mb-6 leading-tight">
       <span class="block mb-2">Discover Premium</span>
       <span class="gradient-text">Nail Beauty</span>
   </h1>
   ```

**Important**: Keep the `<span>` tags and class names exactly as they are. Only change the text between the tags.

---

#### 4. **Hero Subtitle (Description Text)**

**Location**: Lines 76-80
**Current Code**:
```html
<p class="text-xl md:text-2xl text-gray-300 mb-8 max-w-3xl mx-auto leading-relaxed font-light">
    Discover beautiful, professional-grade nail products that make your nails look salon-fresh every single day. Crafted with care, designed for perfection.
</p>
```

**How to Update**:
1. Find the paragraph text using Ctrl+F
2. Replace everything between `<p>` and `</p>` with your new text
3. **Example**:
   ```html
   <p class="text-xl md:text-2xl text-gray-300 mb-8 max-w-3xl mx-auto leading-relaxed font-light">
       Your new description here. Make it compelling and customer-focused.
   </p>
   ```

---

#### 5. **Feature Cards** (The three main features)

**Location**: Lines 129-220

Each feature card has three main parts:

**Feature Title**:
```html
<h3 class="text-2xl font-bold mb-3">Vegan & Cruelty-Free</h3>
```

**Feature Description**:
```html
<p class="text-gray-400 leading-relaxed mb-4">
    Our entire collection is 100% vegan and never tested on animals...
</p>
```

**Feature Checklist Items**:
```html
<li class="flex items-center space-x-2">
    <span>No animal-derived ingredients</span>
</li>
```

**How to Update Feature Cards**:
1. Find the feature title using Ctrl+F
2. Replace the title text
3. Replace the description paragraph
4. Replace each checklist item by finding the `<span>` tags within the list

**Example** (updating the first feature):
```html
<h3 class="text-2xl font-bold mb-3">Your New Feature Title</h3>
<p class="text-gray-400 leading-relaxed mb-4">
    Your new feature description goes here...
</p>
```

---

#### 6. **Testimonials** (Customer Reviews)

**Location**: Lines 400-530

Each testimonial has:
- **Star rating** (visual, usually 5 stars)
- **Review text**
- **Customer name**
- **Customer title/role**

**How to Update a Testimonial**:

1. Find the testimonial using Ctrl+F (search for part of the review text)
2. Replace the review text:
   ```html
   <p class="text-gray-300 mb-6 text-sm leading-relaxed">
       "Your new testimonial text here..."
   </p>
   ```
3. Replace the customer name:
   ```html
   <p class="font-semibold text-white">New Customer Name</p>
   ```
4. Replace the customer title:
   ```html
   <p class="text-sm text-gray-400">New Title/Role</p>
   ```

**To change the star rating**:
- Each star is a separate `<svg>` element
- To show 4 stars instead of 5, delete one `<svg>` block
- To show 3 stars, delete two `<svg>` blocks
- Don't modify the SVG code itself

---

#### 7. **Hero Statistics** (The numbers section)

**Location**: Lines 95-106

```html
<div class="text-center">
    <div class="text-4xl font-bold gradient-text mb-2">100%</div>
    <p class="text-gray-400">Vegan & Cruelty-Free</p>
</div>
```

**How to Update**:
1. Find the statistic using Ctrl+F
2. Replace the number in the large text (e.g., "100%")
3. Replace the description below it

**Example**:
```html
<div class="text-center">
    <div class="text-4xl font-bold gradient-text mb-2">5000+</div>
    <p class="text-gray-400">Happy Customers</p>
</div>
```

---

#### 8. **FAQ Section** (Questions and Answers)

**Location**: Lines 577-730

Each FAQ item has:
- **Question** (in a button)
- **Answer** (hidden by default, shows when clicked)

**How to Update FAQ**:

1. Find the question using Ctrl+F
2. Replace the question text:
   ```html
   <span class="text-lg font-semibold">Your new question here?</span>
   ```
3. Find the corresponding answer (it's in the `<div class="faq-answer">` right after)
4. Replace the answer text:
   ```html
   <div class="faq-answer hidden px-8 pb-6 text-gray-300 leading-relaxed border-t border-gray-700">
       <p>Your new answer text here...</p>
   </div>
   ```

**Example**:
```html
<!-- Question -->
<span class="text-lg font-semibold">How do I apply KCNails polish?</span>

<!-- Answer -->
<div class="faq-answer hidden px-8 pb-6 text-gray-300 leading-relaxed border-t border-gray-700">
    <p>
        Clean your nails thoroughly, apply a base coat, then apply two thin coats of KCNails polish...
    </p>
</div>
```

---

#### 9. **Footer Text**

**Location**: Lines 810-880

The footer contains several text sections:

**Brand Description**:
```html
<p class="text-gray-400 mb-4">Premium ethical nail products for the modern beauty enthusiast.</p>
```

**Footer Links** (Product Links, Company Links, Legal Links):
```html
<li><a href="https://kcnailsukr.com/" class="text-gray-400 hover:text-pink-500 transition-colors duration-300">Shop All</a></li>
```

**Contact Information**:
```html
<a href="mailto:iainhmunro@gmail.com" class="text-white font-semibold hover:text-pink-500 transition-colors duration-300">iainhmunro@gmail.com</a>
```

**How to Update Footer**:
1. Find the text using Ctrl+F
2. Replace the text between tags
3. For email, replace the email address in both the `href="mailto:..."` part AND the visible text

**Example**:
```html
<a href="mailto:newemail@example.com" class="text-white font-semibold hover:text-pink-500 transition-colors duration-300">newemail@example.com</a>
```

---

## Customizing Styles with Tailwind CSS

### What is Tailwind CSS?

Tailwind CSS is a system of pre-made styling classes. Instead of writing traditional CSS code, you add class names to your HTML elements. Each class name applies specific styles.

**Example**:
```html
<div class="bg-blue-500 text-white p-4 rounded-lg">
    This div has a blue background, white text, padding, and rounded corners
</div>
```

### Understanding Tailwind Classes

Tailwind classes follow a pattern: `[property]-[value]`

| Class | What It Does | Example |
|-------|-------------|---------|
| `text-white` | Makes text white | `<p class="text-white">` |
| `bg-gray-900` | Sets background color to gray | `<div class="bg-gray-900">` |
| `p-4` | Adds padding (space inside) | `<div class="p-4">` |
| `m-6` | Adds margin (space outside) | `<div class="m-6">` |
| `rounded-lg` | Rounds corners | `<div class="rounded-lg">` |
| `shadow-lg` | Adds a shadow | `<div class="shadow-lg">` |
| `hover:text-pink-500` | Changes text color on hover | `<a class="hover:text-pink-500">` |
| `md:text-2xl` | On medium screens, makes text larger | `<h1 class="md:text-2xl">` |

### Common Customizations

#### 1. **Change the Primary Color (Pink to Another Color)**

The landing page uses a pink-to-orange gradient. To change this:

**Step 1: Find all instances of the color**

Use Ctrl+F to search for:
- `from-pink-500` (starting color of gradient)
- `to-orange-500` (ending color of gradient)
- `text-pink-500` (pink text)
- `hover:text-pink-500` (pink on hover)

**Step 2: Replace with new colors**

Tailwind color options include:
- `red-500`, `blue-500`, `purple-500`, `green-500`, `yellow-500`, `indigo-500`, etc.

**Example** (changing from pink/orange to purple/blue):

Original:
```html
<div class="bg-gradient-to-r from-pink-500 to-orange-500">
```

Updated:
```html
<div class="bg-gradient-to-r from-purple-500 to-blue-500">
```

**Step 3: Find and replace all instances**

Use your editor's Find & Replace feature (Ctrl+H or Cmd+H):
1. Find: `from-pink-500`
2. Replace with: `from-purple-500`
3. Click "Replace All"
4. Repeat for `to-orange-500` → `to-blue-500`

---

#### 2. **Change Text Size**

Tailwind has predefined sizes: `text-sm`, `text-base`, `text-lg`, `text-xl`, `text-2xl`, `text-3xl`, `text-4xl`, `text-5xl`, `text-6xl`, `text-7xl`

**Example** (making the main headline smaller):

Original:
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold mb-6 leading-tight">
```

Updated:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-6 leading-tight">
```

**Explanation**: 
- `text-4xl` = size on mobile phones
- `md:text-5xl` = size on medium screens (tablets)
- `lg:text-6xl` = size on large screens (desktops)

---

#### 3. **Change Spacing (Padding and Margins)**

Tailwind spacing: `p-1`, `p-2`, `p-4`, `p-6`, `p-8`, `p-12`, `p-16`, `p-24`, etc.

**Example** (adding more space inside a card):

Original:
```html
<div class="p-8">
```

Updated:
```html
<div class="p-12">
```

**Common spacing classes**:
- `p-4` = small padding inside
- `p-8` = medium padding inside
- `p-12` = large padding inside
- `m-4` = small margin outside
- `m-8` = medium margin outside
- `m-12` = large margin outside

---

#### 4. **Change Background Colors**

**Example** (changing the hero section background):

Original:
```html
<section class="relative min-h-screen flex items-center justify-center overflow-hidden pt-20 pb-20">
```

To add a background color:
```html
<section class="relative min-h-screen flex items-center justify-center overflow-hidden pt-20 pb-20 bg-gray-800">
```

**Available colors**: `bg-gray-50`, `bg-gray-100`, `bg-gray-200`, `bg-gray-300`, `bg-gray-400`, `bg-gray-500`, `bg-gray-600`, `bg-gray-700`, `bg-gray-800`, `bg-gray-900`, `bg-gray-950`, etc.

---

#### 5. **Change Border Styles**

**Example** (making feature cards have thicker borders):

Original:
```html
<div class="card-hover bg-gray-800 border border-gray-700 rounded-2xl p-8">
```

Updated:
```html
<div class="card-hover bg-gray-800 border-2 border-gray-700 rounded-2xl p-8">
```

**Border options**:
- `border` = thin border
- `border-2` = thicker border
- `border-4` = even thicker
- `border-gray-700` = border color

---

#### 6. **Change Button Styles**

**Example** (making buttons larger):

Original:
```html
<a href="https://kcnailsukr.com/" class="bg-gradient-to-r from-pink-500 to-orange-500 text-white px-8 py-3 rounded-full font-bold">
```

Updated:
```html
<a href="https://kcnailsukr.com/" class="bg-gradient-to-r from-pink-500 to-orange-500 text-white px-12 py-4 rounded-full font-bold text-lg">
```

**What changed**:
- `px-8` → `px-12` (wider padding left/right)
- `py-3` → `py-4` (taller padding top/bottom)
- Added `text-lg` (larger text)

---

#### 7. **Responsive Design - Making Changes for Different Screen Sizes**

Tailwind lets you specify different styles for different screen sizes:

- `sm:` = small screens (phones)
- `md:` = medium screens (tablets)
- `lg:` = large screens (desktops)
- `xl:` = extra large screens

**Example** (different text size on different devices):

```html
<p class="text-base md:text-lg lg:text-xl">
    This text is base size on phones, larger on tablets, even larger on desktops
</p>
```

**How to add responsive styling**:
1. Add the breakpoint prefix: `md:`, `lg:`, etc.
2. Add the class after the prefix: `md:text-2xl`

**Example** (making a grid responsive):

Original:
```html
<div class="grid grid-cols-1 gap-8">
```

Updated:
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
```

**What this does**:
- `grid-cols-1` = 1 column on phones
- `md:grid-cols-2` = 2 columns on tablets
- `lg:grid-cols-3` = 3 columns on desktops

---

### Practical Exercise: Complete Style Update

Let's say you want to:
1. Change the main color from pink to teal
2. Make the hero section padding larger
3. Change the feature cards to have 4 cards instead of 3

**Step 1: Change Colors**
- Find & Replace: `from-pink-500` → `from-teal-500`
- Find & Replace: `to-orange-500` → `to-cyan-500`
- Find & Replace: `text-pink-500` → `text-teal-500`
- Find & Replace: `hover:text-pink-500` → `hover:text-teal-500`

**Step 2: Increase Hero Padding**

Find this line:
```html
<section class="relative min-h-screen flex items-center justify-center overflow-hidden pt-20 pb-20">
```

Change to:
```html
<section class="relative min-h-screen flex items-center justify-center overflow-hidden pt-32 pb-32">
```

**Step 3: Change Feature Grid from 3 to 4 columns**

Find this line:
```html
<div class="grid grid-cols-1 md:grid-cols-3 gap-8">
```

Change to:
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
```

This creates:
- 1 column on phones
- 2 columns on tablets
- 4 columns on desktops

---

## Fixing and Managing Links

### Understanding Links in HTML

A link is created with the `<a>` tag:

```html
<a href="https://example.com">Click here</a>
```

- `href="..."` tells the browser where to go when clicked
- The text between `<a>` and `</a>` is what the user sees and clicks on

### Types of Links on Your Page

| Link Type | Example | Used For |
|-----------|---------|----------|
| External Link | `href="https://kcnailsukr.com/"` | Links to other websites |
| Internal Link | `href="#features"` | Links to sections on the same page |
| Email Link | `href="mailto:email@example.com"` | Opens email client |
| File Link | `href="privacy.html"` | Links to other files on your server |

---

### Step-by-Step: Finding All Links

**Step 1: Open your HTML file in a text editor**

**Step 2: Use Find (Ctrl+F) to search for `href=`**

This will show you every link in your document.

**Step 3: Review each link**

As you go through each result, ask:
- Is this link correct?
- Does it point to the right place?
- Is it still active?

---

### Current Links in Your Landing Page

#### Navigation Header Links

**Location**: Lines 30-35

```html
<a href="#features" class="text-gray-300 hover:text-white...">Features</a>
<a href="#benefits" class="text-gray-300 hover:text-white...">Benefits</a>
<a href="#testimonials" class="text-gray-300 hover:text-white...">Testimonials</a>
<a href="#faq" class="text-gray-300 hover:text-white...">FAQ</a>
<a href="https://kcnailsukr.com/" class="bg-gradient-to-r...">Shop Now</a>
```

**What These Do**:
- `#features`, `#benefits`, etc. = Jump to that section on the same page
- `https://kcnailsukr.com/` = Go to the shop website

**How to Update**:
- If you want to change the shop URL, find `href="https://kcnailsukr.com/"` and replace it
- The section links (`#features`, `#benefits`) should match the section `id` attributes

---

#### Mobile Menu Links

**Location**: Lines 45-50

These are the same links, but for mobile phones:

```html
<a href="#features" class="block text-gray-300...">Features</a>
<a href="#benefits" class="block text-gray-300...">Benefits</a>
<a href="#testimonials" class="block text-gray-300...">Testimonials</a>
<a href="#faq" class="block text-gray-300...">FAQ</a>
<a href="https://kcnailsukr.com/" class="block bg-gradient-to-r...">Shop Now</a>
```

**Update both the desktop AND mobile versions when making changes.**

---

#### Hero Section CTA Buttons

**Location**: Lines 82-91

```html
<a href="https://kcnailsukr.com/" class="bg-gradient-to-r...">
    <span>Explore Collection</span>
    <svg>...</svg>
</a>

<button class="border-2 border-pink-500...">
    Learn More
</button>
```

**Note**: The "Learn More" button is a `<button>`, not a link. It doesn't currently go anywhere. To make it functional, change it to:

```html
<a href="#features" class="border-2 border-pink-500...">
    Learn More
</a>
```

---

#### Footer Links

**Location**: Lines 820-860

The footer has several categories of links:

**Product Links**:
```html
<li><a href="https://kcnailsukr.com/">Shop All</a></li>
<li><a href="https://kcnailsukr.com/">New Arrivals</a></li>
```

**Company Links**:
```html
<li><a href="#">About Us</a></li>
<li><a href="blog.html">Blog</a></li>
<li><a href="#">Careers</a></li>
<li><a href="#">Contact Us</a></li>
<li><a href="#">Sustainability</a></li>
```

**Legal Links** (These are important!):
```html
<li><a href="privacy.html">Privacy Policy</a></li>
<li><a href="terms.html">Terms of Service</a></li>
<li><a href="#">Cookie Policy</a></li>
<li><a href="#">Return Policy</a></li>
<li><a href="#">Accessibility</a></li>
```

**Contact Links**:
```html
<a href="mailto:iainhmunro@gmail.com">iainhmunro@gmail.com</a>
```

---

### Step-by-Step: Update a Link

**Example: Change the Shop URL**

**Step 1: Find the link**
- Use Ctrl+F to search for `kcnailsukr.com`
- This will show you every instance

**Step 2: Understand what needs changing**
- Count how many times it appears (there are multiple!)
- Decide if you want to change all of them or just specific ones

**Step 3: Replace the URL**

**Option A: Replace just one link**
1. Find the specific link you want to change
2. Select the URL: `https://kcnailsukr.com/`
3. Delete it
4. Type the new URL: `https://mynewshop.com/`

**Option B: Replace all instances**
1. Use Find & Replace (Ctrl+H)
2. Find: `https://kcnailsukr.com/`
3. Replace with: `https://mynewshop.com/`
4. Click "Replace All"

**Step 4: Save your file**
- Press Ctrl+S
- Test the link in your browser

---

### Step-by-Step: Update the Email Link

**Current Location**: Line 844

```html
<a href="mailto:iainhmunro@gmail.com" class="text-white font-semibold hover:text-pink-500 transition-colors duration-300">iainhmunro@gmail.com</a>
```

**Step 1: Find the email link**
- Use Ctrl+F to search for `mailto:`

**Step 2: Update both parts**

You need to change TWO things:
1. The `href="mailto:..."` part
2. The visible email text

**Step 3: Replace the email**

Original:
```html
<a href="mailto:iainhmunro@gmail.com">iainhmunro@gmail.com</a>
```

Updated:
```html
<a href="mailto:newemail@example.com">newemail@example.com</a>
```

**Important**: Make sure both the `href` email and the visible email match!

---

### Step-by-Step: Fix Broken Links

A broken link is one that doesn't work. Here's how to identify and fix them:

**Step 1: Test each link**
- Click every link on your page in a browser
- Note which ones don't work

**Step 2: Identify the problem**

Common issues:
- **Wrong URL**: The website address is incorrect
- **File doesn't exist**: The HTML file (like `privacy.html`) hasn't been created yet
- **Wrong file path**: The file is in a different folder than expected

**Step 3: Fix the link**

**If it's an external link** (to another website):
```html
<!-- Wrong -->
<a href="htp://example.com">Link</a>

<!-- Correct -->
<a href="https://example.com">Link</a>
```

**If it's a file link** (to a page on your site):
```html
<!-- If the file is in the same folder -->
<a href="privacy.html">Privacy Policy</a>

<!-- If the file is in a subfolder called "pages" -->
<a href="pages/privacy.html">Privacy Policy</a>

<!-- If you need to go up one folder -->
<a href="../privacy.html">Privacy Policy</a>
```

**Step 4: Test again**
- Save your file
- Refresh the browser
- Click the link to verify it works

---

### Common Link Issues and Solutions

| Issue | Problem | Solution |
|-------|---------|----------|
| Link goes nowhere | `href="#"` | Replace with actual URL or section ID |
| File not found | `href="file.html"` but file doesn't exist | Create the file or update the path |
| External link doesn't work | Typo in URL | Check the spelling of the website address |
| Section link doesn't work | `href="#about"` but no section with that ID | Add `id="about"` to the section |
| Email link doesn't work | `href="email@example.com"` (missing `mailto:`) | Change to `href="mailto:email@example.com"` |

---

## Creating and Linking Policy Pages

### Why You Need Policy Pages

Policy pages are important for:
- **Legal compliance**: Required by law in many jurisdictions
- **Trust**: Shows customers you take their privacy seriously
- **SEO**: Search engines favor sites with complete information
- **Professional appearance**: Makes your business look legitimate

Your landing page already has links to these pages:
- `privacy.html` - Privacy Policy
- `terms.html` - Terms of Service

But the files don't exist yet. Let's create them.

---

### Step 1: Create the Privacy Policy File

**Step 1a: Open a text editor**
- Use the same editor you use for your HTML file
- Create a new blank document

**Step 1b: Copy this template**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy for KCNails UKR">
    <title>Privacy Policy - KCNails UKR</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
        }
        .gradient-text {
            background: linear-gradient(135deg, #ec4899 0%, #f97316 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-md border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 bg-gradient-to-br from-pink-500 to-orange-500 rounded-full flex items-center justify-center">
                    <i class="fas fa-sparkles text-white text-lg"></i>
                </div>
                <a href="index.html" class="text-2xl font-bold gradient-text">KCNails</a>
            </div>
            <div class="flex items-center space-x-6">
                <a href="index.html" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Home</a>
                <a href="index.html#faq" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">FAQ</a>
                <a href="https://kcnailsukr.com/" class="bg-gradient-to-r from-pink-500 to-orange-500 text-white px-8 py-3 rounded-full font-bold button-primary hover:shadow-lg hover:shadow-pink-500/50">Shop Now</a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-5xl font-bold mb-8">Privacy Policy</h1>
            <p class="text-gray-400 mb-8">Last updated: January 2025</p>

            <div class="space-y-8 text-gray-300 leading-relaxed">
                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">1. Introduction</h2>
                    <p>
                        KCNails UKR ("we," "us," "our," or "Company") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">2. Information We Collect</h2>
                    <p class="mb-4">We may collect information about you in a variety of ways. The information we may collect on the Site includes:</p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li><strong>Personal Data:</strong> Name, email address, phone number, shipping address, and payment information</li>
                        <li><strong>Device Information:</strong> Browser type, IP address, operating system, and pages visited</li>
                        <li><strong>Usage Information:</strong> How you interact with our website and services</li>
                        <li><strong>Cookies:</strong> Information stored on your device to improve your experience</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">3. Use of Your Information</h2>
                    <p class="mb-4">Having accurate information about you permits us to provide you with a smooth, efficient, and customized experience. Specifically, we may use information collected about you via the Site to:</p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li>Process your transactions and send related information</li>
                        <li>Email you regarding your order</li>
                        <li>Fulfill and manage purchases, orders, payments, and other transactions related to our Site</li>
                        <li>Generate a personal profile about you to make future visits to our Site easier</li>
                        <li>Increase the efficiency and operation of our Site</li>
                        <li>Monitor and analyze usage and trends to improve your experience with our Site</li>
                        <li>Send promotional communications (with your consent)</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">4. Disclosure of Your Information</h2>
                    <p class="mb-4">We may share information we have collected about you in certain situations:</p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li><strong>By Law or to Protect Rights:</strong> If required by law or to protect our rights</li>
                        <li><strong>Third-Party Service Providers:</strong> We may share your information with vendors, consultants, and service providers who assist us in operating our website and conducting our business</li>
                        <li><strong>Business Transfers:</strong> Your information may be transferred as part of a merger, acquisition, or sale of assets</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">5. Security of Your Information</h2>
                    <p>
                        We use administrative, technical, and physical security measures to protect your personal information. However, no method of transmission over the Internet is 100% secure. While we strive to use commercially acceptable means to protect your personal information, we cannot guarantee its absolute security.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">6. Contact Us</h2>
                    <p>
                        If you have questions or comments about this Privacy Policy, please contact us at:
                    </p>
                    <p class="mt-4">
                        <strong>Email:</strong> <a href="mailto:iainhmunro@gmail.com" class="text-pink-500 hover:text-pink-400">iainhmunro@gmail.com</a><br>
                        <strong>Address:</strong> London, United Kingdom
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-950 border-t border-gray-800 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400">
                &copy; 2025 KCNails UKR. All rights reserved. 
                <a href="privacy.html" class="text-pink-500 hover:text-pink-400 mx-2">Privacy</a>
                <a href="terms.html" class="text-pink-500 hover:text-pink-400 mx-2">Terms</a>
            </p>
        </div>
    </footer>
</body>
</html>
```

**Step 1c: Save the file**
1. Click File → Save As
2. Name it: `privacy.html`
3. **Important**: Save it in the SAME FOLDER as your `index.html` file
4. Make sure the file type is "HTML" or "All Files" (not .txt)

---

### Step 2: Create the Terms of Service File

**Step 2a: Open a new text editor document**

**Step 2b: Copy this template**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service for KCNails UKR">
    <title>Terms of Service - KCNails UKR</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            scroll-behavior: smooth;
        }
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen', 'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue', sans-serif;
        }
        .gradient-text {
            background: linear-gradient(135deg, #ec4899 0%, #f97316 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-gray-900 bg-opacity-95 backdrop-blur-md border-b border-gray-800">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <div class="w-10 h-10 bg-gradient-to-br from-pink-500 to-orange-500 rounded-full flex items-center justify-center">
                    <i class="fas fa-sparkles text-white text-lg"></i>
                </div>
                <a href="index.html" class="text-2xl font-bold gradient-text">KCNails</a>
            </div>
            <div class="flex items-center space-x-6">
                <a href="index.html" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">Home</a>
                <a href="index.html#faq" class="text-gray-300 hover:text-white transition-colors duration-300 font-medium">FAQ</a>
                <a href="https://kcnailsukr.com/" class="bg-gradient-to-r from-pink-500 to-orange-500 text-white px-8 py-3 rounded-full font-bold button-primary hover:shadow-lg hover:shadow-pink-500/50">Shop Now</a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-gray-900">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-5xl font-bold mb-8">Terms of Service</h1>
            <p class="text-gray-400 mb-8">Last updated: January 2025</p>

            <div class="space-y-8 text-gray-300 leading-relaxed">
                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">1. Agreement to Terms</h2>
                    <p>
                        By accessing and using this website, you accept and agree to be bound by the terms and provision of this agreement. If you do not agree to abide by the above, please do not use this service.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">2. Use License</h2>
                    <p class="mb-4">Permission is granted to temporarily download one copy of the materials (information or software) on KCNails UKR's website for personal, non-commercial transitory viewing only. This is the grant of a license, not a transfer of title, and under this license you may not:</p>
                    <ul class="list-disc list-inside space-y-2 ml-4">
                        <li>Modify or copy the materials</li>
                        <li>Use the materials for any commercial purpose or for any public display</li>
                        <li>Attempt to decompile or reverse engineer any software contained on the website</li>
                        <li>Remove any copyright or other proprietary notations from the materials</li>
                        <li>Transfer the materials to another person or "mirror" the materials on any other server</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">3. Disclaimer</h2>
                    <p>
                        The materials on KCNails UKR's website are provided on an 'as is' basis. KCNails UKR makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties including, without limitation, implied warranties or conditions of merchantability, fitness for a particular purpose, or non-infringement of intellectual property or other violation of rights.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">4. Limitations</h2>
                    <p>
                        In no event shall KCNails UKR or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of the use or inability to use the materials on KCNails UKR's website.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">5. Accuracy of Materials</h2>
                    <p>
                        The materials appearing on KCNails UKR's website could include technical, typographical, or photographic errors. KCNails UKR does not warrant that any of the materials on its website are accurate, complete, or current. KCNails UKR may make changes to the materials contained on its website at any time without notice.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">6. Links</h2>
                    <p>
                        KCNails UKR has not reviewed all of the sites linked to its website and is not responsible for the contents of any such linked site. The inclusion of any link does not imply endorsement by KCNails UKR of the site. Use of any such linked website is at the user's own risk.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">7. Modifications</h2>
                    <p>
                        KCNails UKR may revise these terms of service for its website at any time without notice. By using this website, you are agreeing to be bound by the then current version of these terms of service.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">8. Governing Law</h2>
                    <p>
                        These terms and conditions are governed by and construed in accordance with the laws of the United Kingdom, and you irrevocably submit to the exclusive jurisdiction of the courts located in England.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">9. Contact Information</h2>
                    <p>
                        If you have any questions about these Terms of Service, please contact us at:
                    </p>
                    <p class="mt-4">
                        <strong>Email:</strong> <a href="mailto:iainhmunro@gmail.com" class="text-pink-500 hover:text-pink-400">iainhmunro@gmail.com</a><br>
                        <strong>Address:</strong> London, United Kingdom
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-950 border-t border-gray-800 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-gray-400">
                &copy; 2025 KCNails UKR. All rights reserved. 
                <a href="privacy.html" class="text-pink-500 hover:text-pink-400 mx-2">Privacy</a>
                <a href="terms.html" class="text-pink-500 hover:text-pink-400 mx-2">Terms</a>
            </p>
        </div>
    </footer>
</body>
</html>
```

**Step 2c: Save the file**
1. Click File → Save As
2. Name it: `terms.html`
3. **Important**: Save it in the SAME FOLDER as your `index.html` file
4. Make sure the file type is "HTML" or "All Files" (not .txt)

---

### Step 3: Verify Your Files Are in the Right Place

**Your folder structure should look like this**:

```
your-project-folder/
├── index.html
├── privacy.html
├── terms.html
└── blog.html (optional)
```

**All files must be in the same folder!**

---

### Step 4: Test the Links

**Step 4a: Open your `index.html` file in a browser**

**Step 4b: Scroll to the footer**

**Step 4c: Click the links**
- Click "Privacy Policy"
- Click "Terms of Service"
- Both should open their respective pages

**Step 4d: Test the back links**
- On the privacy page, click "Home" or the KCNails logo
- Should return to the main page

**If the links don't work**:
1. Make sure all three files are in the same folder
2. Make sure the file names are exactly: `index.html`, `privacy.html`, `terms.html`
3. Check that you saved the files as `.html` (not `.txt`)
4. Refresh the browser (Ctrl+R or Cmd+R)

---

### Step 5: Customize Policy Content

The templates provided are generic starting points. You should customize them with your specific information.

**For Privacy Policy, update**:
- Your company name and location
- The types of data you collect
- How you use the data
- Your contact information
- Any specific policies relevant to your business

**For Terms of Service, update**:
- Your company name
- Your specific terms and conditions
- Your refund policy
- Shipping information
- Warranty information
- Your contact information

---

### Step 6: Update Links Throughout Your Site

Now that you have policy pages, make sure all links point to them:

**In the footer** (already done in the templates):
```html
<a href="privacy.html" class="text-pink-500 hover:text-pink-400">Privacy</a>
<a href="terms.html" class="text-pink-500 hover:text-pink-400">Terms</a>
```

**In the header** (optional, but recommended):
You could add these links to your main navigation menu if desired.

**In the CTA section**:
You might want to add text like:
```html
<p class="text-gray-400 mt-4">By shopping with us, you agree to our <a href="privacy.html" class="text-pink-500">Privacy Policy</a> and <a href="terms.html" class="text-pink-500">Terms of Service</a></p>
```

---

## Troubleshooting Common Issues

### Issue 1: Changes Don't Appear When I Refresh

**Problem**: You edited your HTML file, saved it, but the changes don't show up in the browser.

**Solutions**:

1. **Hard Refresh** (clears browser cache):
   - Windows: `Ctrl+Shift+R`
   - Mac: `Cmd+Shift+R`
   - Or: Close the browser completely and reopen it

2. **Check if you saved the file**:
   - Look at your text editor title bar
   - If there's an asterisk (*) or dot next to the filename, you haven't saved
   - Press Ctrl+S to save

3. **Check if you're editing the right file**:
   - Make sure you're editing `index.html`, not a copy
   - Check the file path in your text editor

4. **Check for file encoding**:
   - Some text editors save files in the wrong format
   - Make sure your file is saved as UTF-8
   - In most editors: File → Save with Encoding → UTF-8

---

### Issue 2: Links Don't Work

**Problem**: You click a link but nothing happens or you get an error.

**Solutions**:

1. **Check the href attribute**:
   - Make sure the URL is correct
   - External links should start with `https://`
   - Internal links should match the file name exactly

2. **Check file names match**:
   - If you linked to `privacy.html`, the file must be named exactly `privacy.html`
   - File names are case-sensitive on some systems
   - Check for extra spaces or special characters

3. **Check file location**:
   - All linked files must be in the same folder as `index.html`
   - If a file is in a subfolder, update the path: `subfolder/file.html`

4. **Test with a simple link**:
   - Try linking to a well-known website first: `href="https://google.com"`
   - If that works, the problem is with your specific link

---

### Issue 3: Styles Look Wrong or Colors Are Off

**Problem**: The page doesn't look like it should. Colors are wrong, text is too big, layout is broken.

**Solutions**:

1. **Check if Tailwind CSS loaded**:
   - Right-click the page → "View Page Source"
   - Look for this line: `<script src="https://cdn.tailwindcss.com"></script>`
   - If it's not there, add it to the `<head>` section

2. **Check for typos in class names**:
   - Tailwind class names are very specific
   - `text-white` works, but `text-whites` doesn't
   - Use Ctrl+F to search for the class and verify spelling

3. **Check if you accidentally deleted HTML tags**:
   - Every opening tag needs a closing tag
   - `<div>` needs `</div>`
   - `<p>` needs `</p>`

4. **Check browser compatibility**:
   - Try opening the page in a different browser
   - Clear your browser cache

---

### Issue 4: Mobile Menu Doesn't Work

**Problem**: The hamburger menu icon appears on mobile, but clicking it doesn't open the menu.

**Solutions**:

1. **Check if JavaScript is enabled**:
   - Make sure you didn't accidentally delete the `<script>` section at the bottom
   - The code starting at line 888 is essential

2. **Check for JavaScript errors**:
   - Right-click → "Inspect" → "Console" tab
   - Look for any red error messages
   - These will tell you what's wrong

3. **Check if the mobile menu HTML is intact**:
   - Look for this code around line 45:
     ```html
     <div class="mobile-menu hidden md:hidden bg-gray-800 border-t border-gray-700">
     ```
   - If it's missing, add it back

---

### Issue 5: FAQ Accordion Doesn't Expand

**Problem**: You click an FAQ question, but the answer doesn't appear.

**Solutions**:

1. **Check if JavaScript is working**:
   - Same as Issue 4 above
   - Check the browser console for errors

2. **Check the HTML structure**:
   - Each FAQ item should have this structure:
     ```html
     <div class="faq-item">
         <button class="faq-question">Question here</button>
         <div class="faq-answer hidden">Answer here</div>
     </div>
     ```

3. **Check if the "hidden" class is there**:
   - The answer should start with `class="faq-answer hidden"`
   - The JavaScript will remove the "hidden" class when clicked

---

### Issue 6: Images Don't Show

**Problem**: You see broken image icons instead of pictures.

**Solutions**:

1. **Check the image URL**:
   - For external images (from the internet), make sure the URL is correct
   - Try opening the URL in a new browser tab

2. **Check image paths for local files**:
   - If the image is on your computer, use: `src="images/photo.jpg"`
   - Make sure the folder path is correct
   - Make sure the file name is spelled correctly

3. **Check if the image file exists**:
   - Navigate to your project folder
   - Look for the image file in the location you specified
   - If it's not there, move it to the right location

---

### Issue 7: Text Is Too Small or Too Big

**Problem**: The text size doesn't look right on your device.

**Solutions**:

1. **Check if it's a responsive design issue**:
   - Your page uses different text sizes for different screen sizes
   - What looks right on desktop might look different on mobile
   - This is usually intentional and correct

2. **Adjust text size with Tailwind**:
   - Find the text element
   - Look for classes like `text-lg`, `text-xl`, `text-2xl`
   - Change to a different size: `text-sm`, `text-base`, `text-lg`, etc.

3. **Check browser zoom**:
   - You might have accidentally zoomed in or out
   - Press Ctrl+0 to reset zoom to 100%

---

### Issue 8: Colors Don't Match the Original

**Problem**: You changed colors with Find & Replace, but now it looks wrong.

**Solutions**:

1. **Undo your changes**:
   - Press Ctrl+Z multiple times to undo recent changes
   - Or reload the file without saving

2. **Check all color references**:
   - Tailwind uses colors like `pink-500`, `pink-600`, `pink-400`
   - If you only replaced `pink-500`, the other shades won't match
   - Replace all variations: `pink-400`, `pink-500`, `pink-600`, etc.

3. **Use Find & Replace more carefully**:
   - Test the replacement on one instance first
   - Then use "Replace All" if it looks correct

---

### Issue 9: Links Open in the Same Tab

**Problem**: You want links to open in a new tab, but they don't.

**Solution**:

Add `target="_blank"` to your link:

```html
<!-- Original -->
<a href="https://example.com">Click here</a>

<!-- Opens in new tab -->
<a href="https://example.com" target="_blank">Click here</a>
```

---

### Issue 10: Footer Looks Broken

**Problem**: The footer layout is messed up or text is overlapping.

**Solutions**:

1. **Check if you accidentally deleted footer content**:
   - The footer should have multiple columns
   - Look for the `<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4">`

2. **Check if footer links are properly formatted**:
   - Each link should be in an `<li>` tag
   - Each `<li>` should be inside a `<ul>` tag

3. **Check screen size**:
   - Footer layout changes on different screen sizes
   - This is normal and intentional

---

## Best Practices for Maintenance

### Regular Maintenance Checklist

**Monthly**:
- [ ] Test all links to make sure they work
- [ ] Check that the page loads quickly
- [ ] Review text for typos and outdated information
- [ ] Test on mobile devices

**Quarterly**:
- [ ] Update testimonials with new customer reviews
- [ ] Update statistics (number of customers, etc.)
- [ ] Review and update FAQ section
- [ ] Check for broken external links

**Annually**:
- [ ] Update copyright year in footer
- [ ] Review and update privacy policy
- [ ] Review and update terms of service
- [ ] Consider design updates or refreshes

---

### File Organization Best Practices

**Recommended folder structure**:

```
kcnails-website/
├── index.html (main landing page)
├── privacy.html (privacy policy)
├── terms.html (terms of service)
├── blog.html (blog page, if you have one)
├── images/ (folder for images)
│   ├── logo.png
│   ├── hero-image.jpg
│   └── testimonial-photo.jpg
├── css/ (folder for custom CSS, if needed)
│   └── custom-styles.css
└── js/ (folder for custom JavaScript, if needed)
    └── custom-script.js
```

**Benefits of this structure**:
- Easy to find files
- Easier to backup
- Easier to update
- Professional appearance

---

### Backup Your Files

**Why backup?**
- Protects against accidental deletion
- Protects against computer failure
- Allows you to restore old versions

**How to backup**:

1. **Cloud Storage** (recommended):
   - Google Drive: Upload your files
   - Dropbox: Sync your folder
   - OneDrive: Sync your folder
   - GitHub: Version control and backup

2. **External Hard Drive**:
   - Copy your entire project folder to an external drive
   - Do this monthly or after major updates

3. **Email**:
   - Email your files to yourself
   - Simple but not ideal for large projects

---

### Version Control with Comments

When you make important changes, add comments in your HTML:

```html
<!-- Updated: January 15, 2025 - Changed hero headline -->
<h1>New Headline Here</h1>

<!-- Updated: January 10, 2025 - Added new testimonial from Sarah -->
<div class="testimonial">
    ...
</div>
```

This helps you remember what changed and when.

---

### Performance Optimization Tips

**Make your page load faster**:

1. **Compress images**:
   - Use tools like TinyPNG.com to reduce image file size
   - Smaller files = faster loading

2. **Minimize CSS and JavaScript**:
   - Tailwind CSS is already optimized
   - Remove any unused code

3. **Use a CDN for external resources**:
   - Your page already uses CDN for Tailwind and Font Awesome
   - This is good for performance

4. **Lazy load images**:
   - Add `loading="lazy"` to images below the fold
   - Example: `<img src="image.jpg" loading="lazy" alt="Description">`

---

### SEO Best Practices

**Improve search engine rankings**:

1. **Update meta tags**:
   - `<title>` - Make it descriptive and include keywords
   - `<meta name="description">` - 150-160 characters, compelling

2. **Use descriptive alt text for images**:
   ```html
   <img src="nails.jpg" alt="Professional KCNails polish in pink and coral colors">
   ```

3. **Use heading hierarchy**:
   - `<h1>` for main title (only one per page)
   - `<h2>` for section titles
   - `<h3>` for subsections

4. **Write quality content**:
   - Use relevant keywords naturally
   - Write for your audience, not just search engines
   - Keep content fresh and updated

---

### Accessibility Best Practices

**Make your site usable for everyone**:

1. **Add alt text to all images**:
   ```html
   <img src="image.jpg" alt="Descriptive text about the image">
   ```

2. **Use semantic HTML**:
   - Use `<header>`, `<nav>`, `<main>`, `<footer>` tags
   - Use proper heading hierarchy

3. **Ensure color contrast**:
   - Text should be readable against the background
   - Your page already has good contrast

4. **Make links descriptive**:
   - Instead of: `<a href="#">Click here</a>`
   - Use: `<a href="privacy.html">Read our privacy policy</a>`

5. **Test with keyboard navigation**:
   - Use Tab key to navigate through links
   - All interactive elements should be reachable

---

### Security Best Practices

**Keep your website secure**:

1. **Use HTTPS**:
   - Your shop link uses `https://` (good!)
   - Make sure all external links use `https://`

2. **Validate user input**:
   - If you add forms, validate the data
   - Never trust data from users

3. **Keep software updated**:
   - Update your text editor
   - Update your browser
   - Update any tools you use

4. **Regular security audits**:
   - Check for broken links
   - Check for outdated information
   - Review external links for security

---

## Quick Reference Guide

### Common HTML Tags Used in Your Page

| Tag | Purpose | Example |
|-----|---------|---------|
| `<h1>` to `<h6>` | Headings (h1 is largest) | `<h1>Main Title</h1>` |
| `<p>` | Paragraph of text | `<p>Your text here</p>` |
| `<a>` | Link | `<a href="url">Link text</a>` |
| `<div>` | Container/section | `<div class="container">...</div>` |
| `<span>` | Inline text styling | `<span class="gradient-text">Text</span>` |
| `<button>` | Clickable button | `<button>Click me</button>` |
| `<img>` | Image | `<img src="image.jpg" alt="Description">` |
| `<ul>` | Unordered list | `<ul><li>Item</li></ul>` |
| `<li>` | List item | `<li>Item text</li>` |
| `<section>` | Page section | `<section id="about">...</section>` |

---

### Common Tailwind Classes Used in Your Page

| Class | Purpose | Example |
|-------|---------|---------|
| `text-white` | White text | `<p class="text-white">` |
| `bg-gray-900` | Dark gray background | `<div class="bg-gray-900">` |
| `p-8` | Padding inside | `<div class="p-8">` |
| `m-6` | Margin outside | `<div class="m-6">` |
| `rounded-lg` | Rounded corners | `<div class="rounded-lg">` |
| `shadow-lg` | Drop shadow | `<div class="shadow-lg">` |
| `flex` | Flexbox layout | `<div class="flex">` |
| `grid` | Grid layout | `<div class="grid">` |
| `md:` | Medium screen size | `<div class="md:text-lg">` |
| `hover:` | On mouse hover | `<a class="hover:text-pink-500">` |

---

### Find & Replace Workflow

1. Open Find & Replace: `Ctrl+H` (Windows) or `Cmd+H` (Mac)
2. Enter what you want to find: `old-text`
3. Enter what you want to replace it with: `new-text`
4. Click "Replace" to replace one at a time
5. Click "Replace All" to replace all instances at once
6. Save your file: `Ctrl+S`

---

### Testing Your Changes

After making any changes:

1. **Save the file**: `Ctrl+S`
2. **Refresh the browser**: `Ctrl+R` or `Cmd+R`
3. **Hard refresh** (clear cache): `Ctrl+Shift+R` or `Cmd+Shift+R`
4. **Test on mobile**: Use browser's responsive design mode (`F12` → mobile icon)
5. **Test all links**: Click every link to make sure it works
6. **Check for errors**: Right-click → Inspect → Console tab

---

## Getting Help

### Resources

- **Tailwind CSS Documentation**: https://tailwindcss.com/docs
- **HTML Reference**: https://developer.mozilla.org/en-US/docs/Web/HTML
- **CSS Reference**: https://developer.mozilla.org/en-US/docs/Web/CSS
- **Font Awesome Icons**: https://fontawesome.com/icons

### Text Editors for Editing HTML

- **VS Code** (recommended): https://code.visualstudio.com/ - Free, powerful
- **Sublime Text**: https://www.sublimetext.com/ - Fast, lightweight
- **Atom**: https://atom.io/ - Free, beginner-friendly
- **Notepad++**: https://notepad-plus-plus.org/ - Windows only, simple

### Browser Developer Tools

Press `F12` in any browser to open Developer Tools:
- **Elements/Inspector**: See and edit HTML
- **Console**: See JavaScript errors
- **Network**: See if files are loading
- **Mobile view**: Test responsive design

---

## Final Checklist Before Launch

Before making your site live, verify:

- [ ] All links work (internal and external)
- [ ] All images display correctly
- [ ] Text is spell-checked and proofread
- [ ] Page loads quickly
- [ ] Mobile layout looks good
- [ ] Footer has correct contact information
- [ ] Privacy policy is complete and accurate
- [ ] Terms of service are complete and accurate
- [ ] All social media links are correct
- [ ] Email links are correct
- [ ] Page title is descriptive
- [ ] Meta description is compelling
- [ ] No broken images or missing files
- [ ] No JavaScript errors in console
- [ ] Tested in multiple browsers
- [ ] Tested on multiple devices (phone, tablet, desktop)

---

## Conclusion

You now have a comprehensive understanding of how to maintain and customize your KCNails landing page. Remember:

- **Start small**: Make one change at a time
- **Test thoroughly**: Always test changes before considering them final
- **Keep backups**: Regularly backup your files
- **Stay organized**: Keep your files in a logical structure
- **Read error messages**: They usually tell you exactly what's wrong
- **Don't be afraid to experiment**: You can always undo changes

The most important thing is to take your time and be methodical. Web development is a skill that improves with practice. Good luck with your KCNails website!