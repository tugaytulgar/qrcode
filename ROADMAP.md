# Local QR Generator - Project Roadmap

A professional, 100% offline, and portable QR code generation suite designed for IT tracking and high-quality textile embroidery.

## Phase 1: Core Engine & Offline Architecture
- [ ] **Single-File Structure:** Build everything within one `index.html` (HTML/CSS/JS).
- [ ] **Zero-Dependency Policy:** Embed all libraries (e.g., qrcode.js) directly into the file. No CDNs.
- [ ] **Real-time Generation:** Implement live-preview as the user types unique codes.
- [ ] **Default Reliability:** Set Error Correction Level to 'H' (High - 30% damage recovery) by default.

## Phase 2: Professional Export & Industrial Standards
- [ ] **Vector Export (SVG):** Implement sharp, scalable vector output for embroidery machines.
- [ ] **Raster Export:** PNG and JPEG with high-resolution scaling (300+ DPI).
- [ ] **Smart File Naming:** Automatically name files based on input text (e.g., `abc1234.png`).
- [ ] **Document Mode:** Generate print-ready PDFs (A4 or Label sizes).

## Phase 3: Textile & Embroidery Optimization
- [ ] **Inversion Mode:** One-click toggle for "White on Black" (Essential for dark hoodies).
- [ ] **Quiet Zone Visualizer:** Visual safety margins to prevent stitching errors near edges.
- [ ] **Styling Suite:**
    - Customize "Eye" shapes (Square, Rounded, or Dot).
    - Customize Body patterns (Liquid, Dots, or Standard).
- [ ] **Contrast Verification:** Ensure 100% black/white ratio for machine scanning.

## Phase 4: Automation & Productivity
- [ ] **Bulk Generator:** Multi-line text input to generate hundreds of unique codes at once.
- [ ] **Zip Export:** Package bulk-generated codes into a single ZIP file (using JSZip).
- [ ] **Local History:** Persistence using `localStorage` to keep the last 20 generated codes.
- [ ] **Scanability Score:** AI-based feedback on the complexity and scan-readiness of the code.

## Phase 5: Mobile & UX Refinement
- [ ] **Mobile-First Responsive UI:** Optimized layout for tablets and phones.
- [ ] **Dark/Light Mode:** System-adaptive UI for the application itself.
- [ ] **Copy to Clipboard:** Direct "Copy Image" functionality for quick pasting into design tools.