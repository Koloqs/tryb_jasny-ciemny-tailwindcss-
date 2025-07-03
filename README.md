# Dark/Light Mode Toggle with TailwindCSS v4

A simple demonstration of implementing dark and light mode switching using TailwindCSS v4 with custom variants.

## 🌟 Features SFAFSFAFS SFASF

- ✅ Dark/Light mode toggle functionality
- ✅ Respects system color scheme preference
- ✅ Custom TailwindCSS dark variant implementation
- ✅ Responsive design
- ✅ Clean, semantic HTML structure

## 🖼️ Screenshots

| Light Mode | Dark Mode |
|------------|-----------|
| ![Light Mode](https://github.com/user-attachments/assets/9c197fb1-8394-4a1c-8234-db7d6ffc087b) | ![Dark Mode](https://github.com/user-attachments/assets/959e2f3a-4519-4172-900a-106be85b4b62) |

## 🚀 Quick Start

1. Clone the repository:
   ```bash
   git clone https://github.com/Koloqs/tryb_jasny-ciemny-tailwindcss-.git
   cd tryb_jasny-ciemny-tailwindcss-
   ```

2. Open `indexx.html` in your browser:
   ```bash
   # Using Python's built-in server
   python3 -m http.server 8000
   # Then open http://localhost:8000/indexx.html
   
   # Or directly open the file
   open indexx.html  # macOS
   start indexx.html # Windows
   ```

## 🛠️ Technical Implementation

### Custom Dark Variant

This project uses a custom TailwindCSS variant for dark mode:

```css
@custom-variant dark (&:where([data-theme=dark], [data-theme=dark] *));
```

This approach uses a `data-theme="dark"` attribute on the HTML element instead of the default `dark:` class-based approach.

### Theme Switching Logic

The JavaScript implementation:
- Detects system color scheme preference on page load
- Toggles between light and dark modes
- Updates button text dynamically
- Uses `data-theme` attribute for theme persistence

## 📁 Project Structure

```
.
├── indexx.html     # Main HTML file
├── input.css       # TailwindCSS input with custom variants
├── output.css      # Generated TailwindCSS output
└── README.md       # This file
```

## 🎨 Customization

### Adding New Dark Mode Styles

Use the custom `dark:` variant in your HTML:

```html
<div class="bg-white dark:bg-slate-900 text-black dark:text-white">
  Content that adapts to both themes
</div>
```

### Modifying Colors

Edit the TailwindCSS color variables in `input.css` or extend the theme configuration.

## 🔧 Development

To modify the styles:

1. Edit `input.css`
2. Rebuild the CSS using TailwindCSS CLI:
   ```bash
   npx tailwindcss -i input.css -o output.css --watch
   ```

## 📝 Browser Support

- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Related Resources

- [TailwindCSS v4 Documentation](https://tailwindcss.com/docs)
- [Dark Mode Best Practices](https://web.dev/prefers-color-scheme/)
- [CSS Custom Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/--*)
