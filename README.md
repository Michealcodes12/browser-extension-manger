# Browser Extensions Manager UI

![Design preview for the Browser extensions manager UI coding challenge](./preview.jpg)

## Welcome! 👋

This is a responsive, dark-mode native Browser Extension Manager UI built dynamically with modern frontend workflows using Vanilla JS, HTML, and CSS. The goal of this project was to replicate a high-fidelity web interface, optimizing interactions and layout across both mobile and desktop screens.

## 🚀 Features

- **Responsive Grid**: Automatically adapting 3-column masonry grid on Destkop, scaling elegantly into a mobile list view without media query compromises.
- **Dynamic Content Architecture**: Content elements are populated asynchronously using the `fetch` API directly from our locally mocked `data.json`.
- **Dynamic Checkboxes Toggle**: Smooth animated states toggling an extension as active or inactive and triggering Toastify alerts. 
- **Tab Filtering Mechanism**: A built-in category sorter immediately shifting between active and inactive states. 
- **Interactive Delete Flow**: We replaced native `window.confirm()` calls with a non-blocking HTML modal, allowing you to fluidly remove an extension from your list exactly as designed without blocking other scripts.
- **Theme Switcher**: An integrated light/dark mode switch.

## 🛠 Built With

- Semantic HTML5 markup
- CSS custom properties (Variables)
- Flexbox and CSS Grid
- Vanilla JavaScript
- [Toastify-JS](https://apvarun.github.io/toastify-js/) - for toast notifications

## 💡 What I Learned

During building this project, several JavaScript techniques were put to practice including:
1. **Event Delegation**: Instead of mapping `change` or `click` event listeners to multiple items created at runtime, we bound a unified event listener to the parent `.cards` div. 
2. **Pathing resolutions**: We successfully mitigated relative path retrieval on our local build architecture via modifying `fetch("./data.json")`. 
3. **Modal Focus Management**: Implemented an application-level floating window interface with complete design parity over basic confirm prompts.

## ⚙ How to Run Locally

If you'd like to test the features above out or build upon it further:

1. Clone or download the repository to your local machine.
2. Ensure you have an HTTP Server setup (If you're using VSCode, the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) Extension is perfect). Do not just double-click the `index.html` file, because the JavaScript utilizes the `fetch()` API which is generally blocked on the `file:///` protocol by web-browsers to prevent CORS/Security issues.
3. Once running via a localhost port, browse to `index.html` within your browser.

## 📸 Screenshots


![Design preview for the Browser extensions manager UI coding challenge](./design/desktop-design-light-active.jpg)

![Design preview for the Browser extensions manager UI coding challenge](./design/desktop-design-dark-active.jpg)



