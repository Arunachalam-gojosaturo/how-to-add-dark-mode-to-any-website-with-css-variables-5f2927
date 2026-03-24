# How to automatically switch to dark mode based on the user's system preferences

_Use the `prefers-color-scheme` media query to automatically switch to dark mode_

## Steps

1. Add a media query to the CSS file to apply the dark theme when the user's system prefers dark mode: `@media (prefers-color-scheme: dark) { :root { --background-color: #333; --text-color: #fff; } }`
2. Test the media query in different browsers and devices to ensure compatibility
3. Use JavaScript to detect the user's system preferences and apply the dark theme accordingly: `const isDarkMode = window.matchMedia('(prefers-color-scheme: dark)').matches; if (isDarkMode) { document.body.classList.add('dark'); }`
4. Add a fallback for older browsers that do not support the `prefers-color-scheme` media query
5. Test the automatic dark mode switching in different browsers and devices to ensure compatibility

## Pitfalls

- Forgetting to add a fallback for older browsers
- Not testing the automatic dark mode switching in different browsers and devices