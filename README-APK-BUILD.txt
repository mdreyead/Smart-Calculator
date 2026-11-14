# Smart Calculator Pro — Android-ready web app

This project is a refreshed, mobile-first version of your uploaded Smart Calculator.

## Included
- Responsive calculator UI for phone screens
- Dark/light theme with saved preference
- BigInt exact whole-number arithmetic (+, -, ×, positive integer powers)
- Scientific functions, DEG/RAD, memory buttons
- Calculation history saved locally
- PWA manifest and service worker for offline caching after first load

## Important: APK build
This ZIP is a web app project, not a compiled APK. A signed Android APK must be built by an Android wrapper/build service.

### Phone-only route (no PC)
1. Upload this project to a GitHub repository (keep `index.html`, `manifest.webmanifest`, and `sw.js` at the repository root).
2. In the repository, open Settings → Pages → deploy from the `main` branch and `/ (root)`.
3. Wait until GitHub Pages gives you an HTTPS website URL.
4. Open PWABuilder (https://www.pwabuilder.com/) in Chrome and enter that URL.
5. Follow its Android package flow. Review package details and signing options before generating.
6. Download the generated APK/AAB if the current PWABuilder flow offers it, then install the APK on your phone. Android may ask you to allow installs from Chrome.

If you only want to use it on your phone without an APK, open the GitHub Pages URL in Chrome → menu → Add to Home screen / Install app.

## Notes
- This calculator's large integer arithmetic is exact for whole-number addition, subtraction, multiplication and positive integer powers. Decimal/scientific and trig operations use JavaScript Number precision.
- Offline caching starts after the first successful website load.
- Do not publish secrets or private API keys in this project.
