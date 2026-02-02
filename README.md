# KH&CO | Master Carpentry & Custom Commissions

A premium, high-conversion portfolio website for **KH&CO**, a division of ThokeGroup. This site is designed to showcase 30 years of master woodworking and capture high-end bespoke commissions.

## 🪵 Brand Aesthetic
The site utilizes a "Heritage Industrial" design language:
- **Primary Colors:** Dark Wood (#543D2D), Deep Oak (#8B4513).
- **Accents:** Industrial Silver and Sandy Brown.
- **Typography:** Playfair Display (Serif) for authority; Inter (Sans-serif) for modern clarity.

## 🚀 Features
- **Dynamic Services Grid:** Services are managed via a JavaScript object array for easy updates without touching HTML structure.
- **Mobile-First Responsive Design:** Clean, single-column layout for mobile users with optimized touch targets.
- **Serverless Inquiry System:** Uses a robust `mailto:` implementation that handles special characters and line breaks without requiring a paid backend.

## 🛠️ Technical Implementation

### Form Handling
To keep overhead at $0, the contact form uses the `mailto:` protocol. 
- **Encoding:** Uses `encodeURIComponent()` to ensure project details with spaces and symbols don't break the link.
- **UX:** Includes a `setTimeout` to reset the form after the email client opens, keeping the landing page clean.

### Mobile Optimization
- **iOS Zoom Fix:** Input font sizes are locked at `16px` to prevent iPhones from forced-zooming when a user taps a field.
- **Grid Collapse:** Uses `grid-template-columns: 1fr !important` for devices under `768px`.

## 📁 Project Structure
```text
├── index.html          # Core structure, styles, and logic
└── assets/             # Photography and brand assets
    ├── kitchenUnit.jpg
    ├── floatingTVStands.jpg
    ├── photobooths.jpg
    └── [etc...]
