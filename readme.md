<div align="center">

# 🍽️ The Urban Table

### *Where traditional flavours meet modern places*

A warm, elegant, fully responsive restaurant website with a dark-chocolate and gold theme, built with pure **HTML5** and **CSS3**. No frameworks, no build step, no JavaScript.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Google Fonts](https://img.shields.io/badge/Google%20Fonts-4285F4?style=for-the-badge&logo=googlefonts&logoColor=white)
![Font Awesome](https://img.shields.io/badge/Font%20Awesome-7.3.1-528DD7?style=for-the-badge&logo=fontawesome&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Desktop%20%7C%20Tablet%20%7C%20Mobile-D9B36F?style=for-the-badge)
![No JS](https://img.shields.io/badge/JavaScript-None-3B2418?style=for-the-badge)

</div>

---

## 📑 Table of Contents

1. [Overview](#-overview)
2. [Pages & Sections](#-pages--sections)
3. [Design System](#-design-system)
   - [Color Palette](#-color-palette)
   - [Typography](#-typography)
   - [Icons](#-icons)
   - [Buttons](#-buttons)
   - [Layout & Spacing](#-layout--spacing)
   - [Animations & Hover Effects](#-animations--hover-effects)
4. [Responsive Design](#-responsive-design)
5. [External Resources (CDN)](#-external-resources-cdn)
6. [Project Structure](#-project-structure)
7. [Getting Started](#-getting-started)
8. [Reservation Form Fields](#-reservation-form-fields)
9. [Known Issues & Future Improvements](#-known-issues--future-improvements)
10. [Author](#-author)

---

## ✨ Overview

**The Urban Table** is a two-page restaurant website:

| Page | File | Purpose |
|---|---|---|
| **Home** | `index.html` | Landing page with hero, about, hot-selling dishes, food gallery, chefs, reviews, booking banner and footer |
| **Reservation** | `reservation.html` | Table booking form with a "Plan Your Visit" info sidebar |

The visual identity is built around a **dark espresso-brown background** with **antique-gold accents**, combined with **calligraphy script headings** and clean sans-serif body text. The result feels like a candle-lit, upscale dining room.

**Tagline:** *"Where tradional flavours meet modern places"* (hero) · *"Where Every Bite Tells a Story."* (footer)

---

## 🧭 Pages & Sections

### 🏠 `index.html`

| # | Section | Anchor / Class | Description |
|---|---|---|---|
| 1 | **Navbar** | `.navbar` | Logo (150×150), site title *"The URBAN Table"* and six nav links |
| 2 | **Hero** | `header` / `.hero_sec` | Full-height (100vh) background photo with 40% black overlay, title, tagline and two CTA buttons (**Menu**, **Reserve your Table**) |
| 3 | **About Us** | `#about` | Image with offset brown backing block, "Our Story" paragraph, and four stat icons |
| 4 | **Hot Selling Items** | `#hotselling` | Three hover-lift dish cards |
| 5 | **The Culinary Canvas** | `#gallery` | 13-image masonry-style gallery (CSS columns) |
| 6 | **Meet Our Chefs** | `#chef` | Two alternating (zig-zag) chef profile cards with quotes |
| 7 | **What People Say** | `#review` | Three testimonial cards with star ratings and avatar initials |
| 8 | **Book Your Table** | `.booking-banner` | Parallax banner with call-to-action |
| 9 | **Footer** | `#contact` | 4-column footer: brand, explore links, opening hours, contact |

**Navigation links:** Home · About · Food Gallery · Our Chefs · Reviews · Contact

#### About Us – stat counters

| Icon | Label |
|---|---|
| 📅 `fa-regular fa-calendar` | 40+ years |
| 🍴 `fa-solid fa-utensils` | 30+ Dishes |
| ⭐ `fa-solid fa-star` | 4.8 Rating |
| 👥 `fa-solid fa-people-line` | 10k+ Guests |



### 📅 `reservation.html`

- **Header:** logo (100px) + "← Back to Home" link
- **Heading block:** *"A table is waiting for you"* → **Book Your Table** → *"Good food, great company and lovely memories."*
- **Booking form card** (left, `2fr`) and **Plan Your Visit** info card (right, `1fr`)
- **Footer:** *"© 2026 The Urban Table. Good food, great company, unforgettable moments."*

---

## 🎨 Design System

### 🌈 Color Palette

The palette is a monochromatic **chocolate-brown → gold → cream** scheme.

#### Backgrounds

| Swatch | Hex | Used for |
|---|---|---|
| ![#5C3A21](https://img.shields.io/badge/-%235C3A21-5C3A21?style=flat-square) | `#5C3A21` | Page background gradient (start, left) |
| ![#1C100B](https://img.shields.io/badge/-%231C100B-1C100B?style=flat-square) | `#1C100B` | Page background gradient (end, right) |
| ![#1c100a](https://img.shields.io/badge/-%231c100a-1c100a?style=flat-square) | `#1c100a` | Footer background |
| ![#2A2420](https://img.shields.io/badge/-%232A2420-2A2420?style=flat-square) | `#2A2420` | Hot-selling dish card background |
| ![#634728](https://img.shields.io/badge/-%23634728-634728?style=flat-square) | `#634728` | Offset block behind About image |
| ![#5A4A35](https://img.shields.io/badge/-%235A4A35-5A4A35?style=flat-square) | `#5A4A35` | Nav link hover background |
| ![#2c1a11](https://img.shields.io/badge/-%232c1a11-2c1a11?style=flat-square) | `#2c1a11` | Reservation page background |
| ![#3b2418](https://img.shields.io/badge/-%233b2418-3b2418?style=flat-square) | `#3b2418` | Reservation cards; dark text on gold buttons |
| ![#29180f](https://img.shields.io/badge/-%2329180f-29180f?style=flat-square) | `#29180f` | Form input background |

> **Main background:** `linear-gradient(to right, #5C3A21, #1C100B)`

#### Gold & Accent Colors

| Swatch | Hex | Used for |
|---|---|---|
| ![#d9b36f](https://img.shields.io/badge/-%23d9b36f-d9b36f?style=flat-square) | `#d9b36f` | **Primary brand gold**: headings, borders, buttons, labels, dividers |
| ![#e5bd7b](https://img.shields.io/badge/-%23e5bd7b-e5bd7b?style=flat-square) | `#e5bd7b` | Chef names, reviewer names, card headings |
| ![#e2bd7c](https://img.shields.io/badge/-%23e2bd7c-e2bd7c?style=flat-square) | `#e2bd7c` | "Meet Our Chefs" heading |
| ![#b68c50](https://img.shields.io/badge/-%23b68c50-b68c50?style=flat-square) | `#b68c50` | "About Us" heading, footer top border |
| ![#D4AF6A](https://img.shields.io/badge/-%23D4AF6A-D4AF6A?style=flat-square) | `#D4AF6A` | "Our Story" subheading |
| ![#e7b84f](https://img.shields.io/badge/-%23e7b84f-e7b84f?style=flat-square) | `#e7b84f` | Review star ratings |
| ![#f7c306](https://img.shields.io/badge/-%23f7c306-f7c306?style=flat-square) | `rgb(247,195,6)` | Dish names on cards |
| ![goldenrod](https://img.shields.io/badge/-goldenrod-DAA520?style=flat-square) | `goldenrod` (`#DAA520`) | Navbar title, hero heading & tagline |
| ![gold](https://img.shields.io/badge/-gold-FFD700?style=flat-square) | `gold` (`#FFD700`) | About-section stat icons |
| ![orange](https://img.shields.io/badge/-orange-FFA500?style=flat-square) | `orange` (`#FFA500`) | Hero button borders & hover fill |
| ![#e4c58e](https://img.shields.io/badge/-%23e4c58e-e4c58e?style=flat-square) | `#e4c58e` | Booking banner subtitle |
| ![#f3d49b](https://img.shields.io/badge/-%23f3d49b-f3d49b?style=flat-square) | `#f3d49b` | Booking button hover text |
| ![#f0d7a8](https://img.shields.io/badge/-%23f0d7a8-f0d7a8?style=flat-square) | `#f0d7a8` | Reservation page title & labels |
| ![#e2c79e](https://img.shields.io/badge/-%23e2c79e-e2c79e?style=flat-square) | `#e2c79e` | Reservation subtitle |
| ![#30190f](https://img.shields.io/badge/-%2330190f-30190f?style=flat-square) | `#30190f` | Hero button hover text |

#### Text Colors (Cream & Warm Neutrals)

| Swatch | Hex | Used for |
|---|---|---|
| ![white](https://img.shields.io/badge/-white-FFFFFF?style=flat-square) | `white` | Nav links, About paragraph, stat labels |
| ![#fff0d5](https://img.shields.io/badge/-%23fff0d5-fff0d5?style=flat-square) | `#fff0d5` | "Book Your Table!" banner heading |
| ![#f5e8d8](https://img.shields.io/badge/-%23f5e8d8-f5e8d8?style=flat-square) | `#f5e8d8` | Banner paragraph |
| ![#f5ead8](https://img.shields.io/badge/-%23f5ead8-f5ead8?style=flat-square) | `#f5ead8` | Reservation body text |
| ![#f2e6d6](https://img.shields.io/badge/-%23f2e6d6-f2e6d6?style=flat-square) | `#f2e6d6` | Chef description text |
| ![#f0e4d5](https://img.shields.io/badge/-%23f0e4d5-f0e4d5?style=flat-square) | `#f0e4d5` | Review text |
| ![#e9d8c0](https://img.shields.io/badge/-%23e9d8c0-e9d8c0?style=flat-square) | `#e9d8c0` | Footer base text |
| ![#e8d8c5](https://img.shields.io/badge/-%23e8d8c5-e8d8c5?style=flat-square) | `#e8d8c5` | "Hot Selling" subtitle |
| ![#e8d5b7](https://img.shields.io/badge/-%23e8d5b7-e8d5b7?style=flat-square) | `#e8d5b7` | Section subtitles (chefs, reviews) |
| ![#d5c3ad](https://img.shields.io/badge/-%23d5c3ad-d5c3ad?style=flat-square) | `#d5c3ad` | "Plan Your Visit" body text |
| ![#c8b5a1](https://img.shields.io/badge/-%23c8b5a1-c8b5a1?style=flat-square) | `#c8b5a1` | Reviewer role |
| ![#c7b6a3](https://img.shields.io/badge/-%23c7b6a3-c7b6a3?style=flat-square) | `#c7b6a3` | Footer links & descriptions |
| ![#bba58c](https://img.shields.io/badge/-%23bba58c-bba58c?style=flat-square) | `#bba58c` | Placeholders, reservation footer |
| ![#a99783](https://img.shields.io/badge/-%23a99783-a99783?style=flat-square) | `#a99783` | Footer copyright |

#### Borders, Overlays & Transparent Layers

| Value | Used for |
|---|---|
| `rgba(0, 0, 0, 0.4)` | Hero image dark overlay |
| `rgba(25, 13, 7, 0.55)` → `rgba(25, 13, 7, 0.65)` | Booking banner gradient overlay |
| `rgba(255, 255, 255, 0.035)` | Chef card glass background |
| `rgba(255, 255, 255, 0.045)` | Review card glass background |
| `rgba(217, 179, 111, 0.2)` | Chef card border (default) |
| `rgba(217, 179, 111, 0.3)` | Review card border (default) |
| `rgba(217, 179, 111, 0.25)` | Reviewer divider line |
| `rgba(217, 179, 111, 0.65)` | Chef card border (hover) |
| `rgba(0, 0, 0, 0.35)` / `0.3` / `0.25` | Hover box-shadows |
| `#725337` | Reservation navbar/footer divider |
| `#80613d` | Reservation card & input borders |
| `brown` (`#A52A2A`) | Legacy `.card h4` button style |

---

### 🔤 Typography

#### Google Fonts (loaded in `index.html`)

```html
<link href="https://fonts.googleapis.com/css2?family=Alex+Brush&family=Italianno&family=DM+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
```

| Font | Type | Weights | Where it's used |
|---|---|---|---|
| **[Alex Brush](https://fonts.google.com/specimen/Alex+Brush)** | Script / calligraphy | 400 | "About Us", "The Culinary Canvas", "Meet Our Chefs", chef names, "What People Say", "Book Your Table!", footer brand name, reviewer avatar letters |
| **[Italianno](https://fonts.google.com/specimen/Italianno)** | Script / handwritten | 400 | "Hot Selling" subtitle, chef quotes, footer tagline, footer hours note |
| **[DM Sans](https://fonts.google.com/specimen/DM+Sans)** | Sans-serif | 400, 500, 600, 700 | Loaded, available for future use |
| **[Ballet](https://fonts.google.com/specimen/Ballet)** | Script / formal | 400 | Referenced in CSS for **"URBAN"** in the logo title and the **"HOT SELLING ITEMS"** heading, with `cursive` fallback |

> ⚠️ **Note:** `Ballet` is referenced in `style.css` but is not included in the Google Fonts `<link>`, so those two headings currently render with the browser's default `cursive` font. See [Known Issues](#-known-issues--future-improvements).

#### System / Web-Safe Fonts

| Font stack | Where it's used |
|---|---|
| `Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif` | Navbar title "The Urban Table" |
| `'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif` | Hero heading "THE URBAN TABLE" |
| `Georgia, serif` | Hero buttons, footer column headings, quote mark, reservation headings and info text |
| `Cambria, Cochin, Georgia, Times, 'Times New Roman', serif` | About-section stat labels |
| `'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif` | Dish card names |
| `'Trebuchet MS', sans-serif` | Chef bios, review text, banner paragraph, footer description |
| `Arial, sans-serif` | Small uppercase eyebrow labels, reservation form & body |

#### Type Scale (Desktop)

| Element | Font | Size | Notes |
|---|---|---|---|
| Navbar title | Impact | `50px` | `goldenrod` |
| Nav links | Default | `20px` | white, `8px 20px` padding |
| Hero `h1` | Lucida Sans | `50px` | |
| Hero tagline | Default | `30px` | |
| Hero buttons | Georgia | `20px` | |
| About heading | Alex Brush | `40px` | `#b68c50` |
| "Our Story" | Default | `1.8rem` | `#D4AF6A` |
| About paragraph | Default | `1.4rem` | justified |
| Hot Selling heading | Ballet | `37px` | (overrides `75px`) |
| Hot Selling subtitle | Italianno | `30px` | |
| Dish card name | Trebuchet MS | `25px` | weight `800` |
| Gallery heading | Alex Brush | `45px` | |
| Eyebrow labels | Arial | `13px` | `letter-spacing: 5px` |
| Chefs / Reviews heading | Alex Brush | `65px` | |
| Chef name | Alex Brush | `48px` | |
| Chef role | Default | `12px` | `letter-spacing: 4px`, bold |
| Chef bio | Trebuchet MS | `17px` | `line-height: 1.8` |
| Chef quote | Italianno | `30px` | `line-height: 1.3` |
| Review text | Trebuchet MS | `16px` | `line-height: 1.8` |
| Review stars | Default | `23px` | `letter-spacing: 4px` |
| Quote mark `“` | Georgia | `85px` | 80% opacity |
| Reviewer name | Default | `17px` | |
| Banner heading | Alex Brush | `85px` | |
| Banner paragraph | Trebuchet MS | `17px` | |
| Footer brand | Alex Brush | `48px` | |
| Footer tagline | Italianno | `27px` | |
| Footer column heading | Georgia | `18px` | |
| Footer links | Default | `14px` | |
| Copyright | Default | `12px` | |
| Reservation `h1` | Georgia | `48px` | |
| Reservation subtitle | Georgia italic | `17px` | `letter-spacing: 1px` |
| Reservation card `h2` | Georgia | `25px` | |
| Form labels / inputs | Arial | `14px` | |

---

### 🔣 Icons

| Source | Version | Style | Usage |
|---|---|---|---|
| **[Font Awesome Free](https://fontawesome.com/)** | `7.3.1` (cdnjs) | Solid + Regular | About-section stats |
| **Unicode characters** | | | Stars `★`, quote `“`, arrow `→` / `←` |
| **Emoji** | | | Footer contact: 📍 📞 ✉️ |

**Font Awesome icons used:**

| Class | Meaning |
|---|---|
| `fa-regular fa-calendar` | Years of experience |
| `fa-solid fa-utensils` | Dishes |
| `fa-solid fa-star` | Rating |
| `fa-solid fa-people-line` | Guests served |

**Icon styling:** color `gold`, size `2rem`, padding `10px`.

---

### 🔘 Buttons

| Button | Class | Style | Hover |
|---|---|---|---|
| **Menu / Reserve your Table** | `.hero-btn` | Transparent, `4px solid orange` border, `50px` radius, `250×50px`, white Georgia 20px | Fills `orange`, text turns `#30190f` (0.3s) |
| **Reserve Your Spot →** | `.booking-btn` | Solid `#d9b36f`, text `#3b2418`, bold 16px, `50px` radius, `15px 35px` padding | Becomes transparent, text `#f3d49b`, lifts `-5px`, arrow slides `+7px` |
| **Book A Table →** | `.footer-reserve` | Text link with `1px solid #d9b36f` underline | Turns white, `letter-spacing: 1px` |
| **Confirm Reservation Request** | `.submit-button` | Full-width, solid `#d9b36f`, text `#2c1a11`, bold 15px, `5px` radius | Becomes transparent with gold text |
| **Nav links** | `.nav-links a` | `8px 20px` padding | Pill background `#5A4A35`, `40px` radius (0.3s) |

---

### 📐 Layout & Spacing

| Section | Technique | Key values |
|---|---|---|
| Global | `box-sizing: border-box`, `scroll-behavior: smooth`, `overflow-x: hidden` | |
| Navbar | Flexbox, `space-between` | `10px` padding |
| Hero | Flexbox column, centered | `100vh` height, `margin-top: 100px` |
| About | Flexbox, `gap: 40px` | Image `600×400`, wrapper width `90%` |
| Hot Selling | Flexbox wrap, `space-between` | Container `90%`, cards `350×550px` (image `400px` tall) |
| Gallery | **CSS multi-column masonry** | `columns: 3`, `column-gap: 25px`, `border-radius: 8px` |
| Chefs | Flexbox, `gap: 65px`; `row-reverse` for alternate | Max-width `1400px`, image `43%` × `350px`, radius `12px`/`15px` |
| Reviews | **CSS Grid** | `repeat(3, 1fr)`, `gap: 30px`, radius `15px` |
| Booking banner | Flexbox centered | `min-height: 500px`, `background-attachment: fixed` (parallax) |
| Footer | **CSS Grid** | `1.5fr 0.8fr 1.2fr 1.2fr`, `gap: 45px`, max-width `1450px` |
| Reservation | **CSS Grid** | `2fr 1fr`, `gap: 25px`, max-width `1150px`; form is a 2-column grid with `gap: 18px` |

---

### 🎬 Animations & Hover Effects

All animations are pure CSS `transition`s. No JavaScript.

| Element | Effect |
|---|---|
| **Dish cards** | `translateY(-15px) rotateX(3deg) rotateY(-2deg)` + deep shadow `0 25px 45px rgba(0,0,0,.35)` (0.4s) |
| **Gallery images** | Zoom `scale(1.06)` in a clipped frame (0.6s) |
| **Chef cards** | Lift `-7px`, border brightens, photo zooms `1.08` + `brightness(1.1)`, gold line grows `90px → 180px` |
| **Review cards** | Lift `-12px`, border becomes solid gold, shadow |
| **Booking button** | Lift + arrow slide |
| **Footer links** | Color change + `padding-left: 8px` slide |
| **Hero buttons / nav links** | Background fill transitions |
| **Smooth scroll** | `scroll-behavior: smooth` on `html` |
| **Parallax banner** | `background-attachment: fixed` (disabled on mobile) |

---

## 📱 Responsive Design

| Breakpoint | Target | Key changes |
|---|---|---|
| **> 1247px** | Desktop | Full layouts as described above |
| **≤ 1247px** | Tablet | Navbar title `40px`; gallery → **2 columns**; chef image `40%` × `300px`; reviews → **2 columns**; banner heading `70px`; footer → **2 columns** |
| **≤ 600px** | Mobile | Navbar stacks vertically (title `20px`); About stacks; dish cards stack; gallery → **1 column**; chefs stack (image `250px` tall); reviews → **1 column**; banner heading `55px`, parallax off; footer → **1 column** |
| **≤ 900px** *(reservation)* | Tablet | Form and info card stack, width `92%` |
| **≤ 600px** *(reservation)* | Mobile | Form fields go single column; heading `36px` |

Viewport meta: `<meta name="viewport" content="width=device-width, initial-scale=1.0">`

---

## 🌐 External Resources (CDN)

| Resource | URL | Purpose |
|---|---|---|
| Google Fonts | `https://fonts.googleapis.com/css2?family=Alex+Brush&family=Italianno&family=DM+Sans:wght@400;500;600;700&display=swap` | Script & sans-serif fonts |
| Font Awesome 7.3.1 | `https://cdnjs.cloudflare.com/ajax/libs/font-awesome/7.3.1/css/all.min.css` | Icons |

> An internet connection is needed on first load so fonts and icons can be fetched. Everything else is local.

---

## 📂 Project Structure

```
theurbantable/
├── index.html              # Home page
├── reservation.html        # Table booking page
├── style.css               # Styles for the home page
├── reservation_style.css   # Styles for the reservation page
└── images/
    ├── logo.png
    ├── restaurant ambience.png
    ├── restaurant in.jpeg
    ├── table.avif
    ├── chef1.avif
    ├── chef2.avif
    ├── ...
    ├── gallery/            # Food gallery photos
    └── menu/               # Menu / dish photos
```

---

## 🚀 Getting Started

No installation or build tools needed.

**Option 1: Open directly**
```bash
git clone https://github.com/Trideep091/theurbantable.git
cd theurbantable
open index.html        # macOS  (Windows: start index.html · Linux: xdg-open index.html)
```

**Option 2: Local server (recommended)**
```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```
Or use the **Live Server** extension in VS Code.

**Option 3: Deploy free**
Push to GitHub, then go to **Settings → Pages → Deploy from branch → `main` / root**.

---

## 📝 Reservation Form Fields

| Field | Type | Required | Options / Placeholder |
|---|---|---|---|
| Full Name | `text` | ✅ | "Enter your name" |
| Phone Number | `tel` | ✅ | "Enter your phone number" |
| Email Address | `email` | ✅ | "Enter your email" |
| Number of Guests | `select` | ✅ | 1 – 8, or "More than 8" |
| Date | `date` | ✅ | Native date picker |
| Time | `select` | ✅ | Lunch: 11:00 AM – 2:30 PM · Dinner: 6:00 PM – 9:30 PM (30-minute slots) |
| Occasion | `select` | Optional | Birthday, Anniversary, Family Gathering, Date Night, Business Dinner, Other |
| Special Requests | `textarea` | Optional | "Any dietary requirements or seating preferences?" |

**Form states:** focus shows a `2px solid #d9b36f` outline; placeholders are `#bba58c`; the textarea is vertically resizable (min-height `100px`).

> The form currently uses `action="#"` and `method="post"`, so it is front-end only. A backend (or a service like Formspree / EmailJS) is needed to receive submissions.

---

## 🛠️ Known Issues & Future Improvements

**Small fixes**
- [ ] Add `Ballet` to the Google Fonts `<link>` (or switch those headings to Alex Brush) so the "URBAN" title and "HOT SELLING ITEMS" render in the intended script font
- [ ] The booking banner button points to `#reservation` (no such anchor); change it to `reservation.html`
- [ ] Typos: "tradional" → "traditional" in the hero tagline, and missing spaces in the chef bio ("andexpertise", "plate.With")
- [ ] Add meaningful `alt` text to the logo and gallery images (accessibility and SEO)
- [ ] `.hero_sec p { text-decoration: italic }` should be `font-style: italic`
- [ ] Replace the placeholder footer address and contact details with real ones
- [ ] Add `Ballet` / `DM Sans` consistently, or remove unused font requests

**Ideas**
- [ ] Hamburger menu for mobile
- [ ] Full menu page using the extra images in `images/menu/`
- [ ] Lightbox for the gallery
- [ ] Form validation and a backend for real reservations
- [ ] Compress images (WebP/AVIF, `loading="lazy"`) to cut the ~17 MB payload
- [ ] Add Open Graph / meta description tags and a favicon

---

## 👤 Author

**Trideep** · GitHub: [@Trideep091](https://github.com/Trideep091)

---

<div align="center">

*© 2026 The Urban Table. Good food, great company, unforgettable moments.* 🍷

</div>