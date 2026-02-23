---
trigger: always_on
---

# Project: Portable Local QR Generator

## 1. Core Principles
- **Offline First:** The application must function entirely offline. No external CDNs (Google Fonts, Bootstrap CDN, etc.) are allowed. All dependencies must be bundled within the HTML file or stored locally.
- **Portability:** The entire application must reside within a single folder (e.g., `C:/temp/QRCode`). It must be fully functional when the folder is moved to another computer.
- **Single-File Architecture:** Aim for a single `index.html` file containing all HTML, CSS (Tailwind/Standard), and JavaScript to ensure maximum portability.
- **No Backend:** The app must run in a standard web browser without requiring a local server (Node.js, Python, etc.), using the `file://` protocol.

## 2. Technical Standards
- **QR Engine:** Use a robust, lightweight JS library (like `qrcode.js` or `bwip-js`).
- **Default Settings:** Set default Error Correction Level to **"H" (High - 30%)** to ensure durability on physical products like textiles.
- **Resolution:** All visual exports (PNG/JPEG) must be generated at high DPI (at least 300 DPI equivalent) for professional printing/embroidery.
- **Mobile-First Design:** Use a responsive UI layout that adapts seamlessly to mobile devices for future-proofing.

## 3. Export Requirements
- **Supported Formats:** PNG, JPEG, SVG (Vector), and PDF.
- **Naming Convention:** Exported files should automatically be named based on the input text/code (e.g., `abc1234.png`).
- **PDF Layout:** PDF export should include the QR code centered on a standard A4 or label-sized page.

## 4. UI/UX Features
- **Live Preview:** Generate the QR code in real-time as the user types.
- **Contrast Check:** Ensure the QR code maintains high contrast (Pure Black on Pure White).
- **History:** Implement a "Recent Codes" list using `localStorage`.
- **Bulk Generation:** Support multi-line input to generate and download multiple QR codes as a ZIP file or sequential downloads.

## 5. Development Constraints
- Use modern ES6+ JavaScript.
- Write clean, commented code in English.
- Ensure the UI is intuitive, clean, and professional.