# Minimal Sticker Loader

A high-performance, aesthetic loading screen built for modern web applications. Featuring a mechanical "odometer-style" rolling percentage counter and an interactive, physics-based sticker trail.

## 🚀 Features

*   **Mechanical Rolling Counter:** A smooth, odometer-style number animation that "rolls" to the next digit using CSS `cubic-bezier` transitions.
*   **Physics-Based Sticker Trail:** An interactive sticker system that follows the cursor with a spring-like delay, utilizing HTML5 Canvas for high-performance rendering.
*   **Minimalist UI:** Designed with a premium agency aesthetic, featuring a bottom-right percentage watermark and a centered call-to-action button.
*   **Responsive Design:** Fully fluid layout using `clamp()` and `vw/vh` units to ensure it looks sharp on any screen size.
*   **Performance Optimized:** Uses `requestAnimationFrame` for the sticker engine and CSS hardware-accelerated transforms for the counter.

## 🛠 Tech Stack

*   **HTML5 / CSS3:** Modern Flexbox layout and CSS animations.
*   **JavaScript (ES6+):** Custom physics engine and DOM manipulation for the rolling tracks.
*   **Canvas API:** High-frequency rendering for the interactive sticker trail.

## 💻 Implementation

1.  **Include the Assets:** Ensure your sticker images are hosted or in your local `/assets` folder.
2.  **Add the Markup:** Place the `#sticker-loader` HTML structure at the top of your `<body>` tag.
3.  **Styles:** Copy the CSS into your stylesheet. Note the usage of `tabular-nums` for the percentage—this is critical to prevent text jittering.
4.  **Init:** The loader initializes automatically on `DOMContentLoaded` and will handle its own `fade-out` class once the progress reaches 100%.

## 🎨 Customization

*   **Stickers:** Modify the `stickerURLs` array in the script to point to your own transparent SVG or PNG assets.
*   **Speed:** Adjust the `progressInterval` in the JavaScript to match your actual asset loading time or API response time.
*   **Aesthetic:** The rolling tracks are built by generating 100 span elements dynamically—if you need to change the font, simply update the `font-family` on the `.loader-percentage-watermark` class.

## 📝 License

This project is open-source. Feel free to use the sticker trail logic in your own production environments.
