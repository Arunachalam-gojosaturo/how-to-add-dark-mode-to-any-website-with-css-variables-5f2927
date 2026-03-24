# How to add a dark mode toggle to a website with a complex layout

_Use a combination of CSS variables and JavaScript to apply the dark theme to different parts of the layout_

## Steps

1. Create a new CSS file and define the light and dark theme variables for each part of the layout: `:root { --header-background-color: #f0f0f0; --header-text-color: #000; }` and `:root.dark { --header-background-color: #333; --header-text-color: #fff; }`
2. Add a class to each part of the layout to apply the dark theme: `document.getElementById('header').classList.toggle('dark');`
3. Use JavaScript to add an event listener to the toggle button: `const toggleButton = document.getElementById('dark-mode-toggle'); toggleButton.addEventListener('click', () => { document.body.classList.toggle('dark'); });`
4. Test the dark mode toggle in different browsers and devices to ensure compatibility
5. Use a CSS preprocessor like Sass or Less to simplify the process of defining and applying the dark theme variables

## Pitfalls

- Forgetting to apply the dark theme to all parts of the layout
- Not testing the dark mode toggle in different browsers and devices