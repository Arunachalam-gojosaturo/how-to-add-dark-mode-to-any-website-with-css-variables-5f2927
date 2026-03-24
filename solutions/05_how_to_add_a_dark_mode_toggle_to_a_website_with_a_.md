# How to add a dark mode toggle to a website with a custom design

_Use a combination of CSS variables, JavaScript, and custom CSS to apply the dark theme to the custom design_

## Steps

1. Create a new CSS file and define the light and dark theme variables for the custom design: `:root { --custom-background-color: #f0f0f0; --custom-text-color: #000; }` and `:root.dark { --custom-background-color: #333; --custom-text-color: #fff; }`
2. Add a class to the custom design elements to apply the dark theme: `document.getElementById('custom-design').classList.toggle('dark');`
3. Use JavaScript to add an event listener to the toggle button: `const toggleButton = document.getElementById('dark-mode-toggle'); toggleButton.addEventListener('click', () => { document.body.classList.toggle('dark'); });`
4. Test the dark mode toggle in different browsers and devices to ensure compatibility
5. Use a custom CSS framework like Bootstrap or Tailwind CSS to simplify the process of defining and applying the dark theme variables

## Pitfalls

- Forgetting to apply the dark theme to all custom design elements
- Not testing the dark mode toggle in different browsers and devices