# How to set up a basic dark mode toggle using CSS variables and JavaScript

_Use CSS variables to define light and dark themes, and JavaScript to toggle between them_

## Steps

1. Create a new CSS file and define the light and dark theme variables: `:root { --background-color: #f0f0f0; --text-color: #000; }` and `:root.dark { --background-color: #333; --text-color: #fff; }`
2. Add a class to the HTML body to apply the dark theme: `document.body.classList.toggle('dark');`
3. Create a toggle button in the HTML: `<button id='dark-mode-toggle'>Toggle Dark Mode</button>`
4. Use JavaScript to add an event listener to the toggle button: `const toggleButton = document.getElementById('dark-mode-toggle'); toggleButton.addEventListener('click', () => { document.body.classList.toggle('dark'); });`
5. Test the dark mode toggle in different browsers and devices to ensure compatibility

## Pitfalls

- Forgetting to add the `:root` selector when defining CSS variables
- Not testing the dark mode toggle in different browsers and devices