# card

**card** is a powerful, web-based layer editor designed for creating custom RPG, Tarot, and trading cards. Built entirely in a single HTML file, it features a robust layer management system, real-time 3D parallax preview, and high-resolution exporting capabilities.

## ✨ Features

*   **Layer-Based Editing:** Add, reorder, hide, delete, and rename multiple layers just like in professional design software.
*   **4 Layer Types:**
    *   **Text:** Supports custom colors, outlines, opacity, and image masking/fills.
    *   **Image:** Upload local images with adjustable dimensions, border radii, and soft-edge blur.
    *   **Box:** Create solid colored or image-filled shapes with customizable borders.
    *   **Gradient:** Generate dynamic linear gradients with adjustable stops and angles.
*   **Massive Typography Library:** Includes 30 unique Google Fonts ranging from Cyberpunk (`Orbitron`, `Rubik Glitch`) and Fantasy (`Uncial Antiqua`, `MedievalSharp`), to Roman (`Marcellus`), Cartoony (`Bangers`), and Thai-supported fonts (`Kanit`, `Chakra Petch`).
*   **True 3D Parallax:** Toggleable 3D tilt effect that calculates Z-depth based on layer hierarchy, making your card elements pop out as you move your mouse.
*   **Persistent Auto-Save:** Automatically saves your progress to your browser's `localStorage`. You will never lose your work if you accidentally refresh or close the tab.
*   **Project Import/Export:** Save your entire workspace as a `.json` file to share with friends or back up your designs, and load them back at any time.
*   **High-Res PNG Export:** Generates clean, high-quality images (744x1039px, standard 6.3cm x 8.8cm card ratio) using `html2canvas`.

## 🚀 Getting Started

Since the application is self-contained in a single file, setup is instantaneous:

1. Clone or download the repository.
2. Double-click `index.html` to open it in any modern web browser (Chrome, Edge, Firefox, or Safari).
3. No build tools, Node.js, or local servers are required!

## 🛠️ How to Use

### The Interface
*   **Preview Canvas (Left):** Shows your card in real-time. Move your mouse over it to see the 3D parallax effect (if enabled).
*   **Layer Editor (Right):** Click `+ ADD LAYER` to add new elements. Click any layer's header to expand its settings. You can reorder layers using the up/down arrows or delete them with the red `X`.
*   **Global Settings (Top Left ⚙️):** Adjust the card's background color, border properties, clipping rules, and toggle the 3D Parallax effect.
*   **Actions (Bottom Left 💾):** Hover over the save disk icon to download your finished PNG, save your project as a JSON file, or load an existing JSON file.

### Advanced Tips
*   **Image Masking:** On Text or Box layers, check "Image Fill / Mask" and upload an image to clip that image strictly inside the text or shape.
*   **Overflow Clipping:** By default, elements outside the card bounds are clipped. If you want a character or effect to break the frame, uncheck "Clip to Card Bounds" in the Global Settings.
*   **Border Z-Index:** You can push the card's physical border behind certain elements (like a character's head) by lowering the Border Z-Index in the settings.

## 📦 Dependencies

This project is built with vanilla HTML, CSS, and JavaScript. It relies on the following external resources via CDN:
*   [Google Fonts](https://fonts.google.com/) for typography.
*   [html2canvas](https://html2canvas.hertzen.com/) (v1.4.1) for rendering the DOM to a downloadable PNG.