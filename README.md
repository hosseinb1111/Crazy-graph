# Crazy Graph

A mesmerizing, real-time glitch animation built with React and HTML5 Canvas.  
Watch as random characters cascade across the screen, shifting colors and creating a digital "glitch" effect with customizable vignettes.

## 🚀 Demo

Simply open the `index.html` file in any modern browser to see the effect in action.  
No build tools or dependencies required—everything is bundled in a single file.

## ✨ Features

- **Dynamic Glitch Canvas**: Random characters (letters, numbers, symbols) continuously update, creating a "Matrix"‑like storm.
- **Smooth Color Transitions**: Each character can transition between random colors with a smooth easing effect.
- **Customizable Speed**: Control the glitch update interval.
- **Vignette Effects**: Optional center and outer vignette overlays for a cinematic feel.
- **Fully Responsive**: Adapts to any container size.
- **Single‑File Deployment**: Just drop the HTML file anywhere—works offline.

## 🎮 How to Use

1. Clone or download the repository.
2. Open the `index.html` file in your web browser.
3. Enjoy the animation!

No installation or server required.

## ⚙️ Customization

The main component accepts several props to tweak the visual experience:

```jsx
<GlitchCanvas
  glitchColors={['#2b4539', '#61dca3', '#61b3dc']}  // Array of color hex strings
  glitchSpeed={50}                                   // Update interval in ms
  centerVignette={true}                              // Inner vignette
  outerVignette={true}                               // Outer vignette
  smooth={true}                                      // Smooth color transitions
  characters="ABCDEFGHIJKLMNOPQRSTUVWXYZ!@#$&*()-_+=/[]{};:<>.,0123456789"
/>
```

**Props**:

| Prop | Type | Default | Description |
|------|------|---------|-------------|
| `glitchColors` | `string[]` | `['#2b4539','#61dca3','#61b3dc']` | Colors used for the characters. |
| `glitchSpeed` | `number` | `50` | Milliseconds between glitch updates. |
| `centerVignette` | `boolean` | `false` | Adds a dark vignette at the center. |
| `outerVignette` | `boolean` | `true` | Adds a dark vignette around the edges. |
| `smooth` | `boolean` | `true` | Enables smooth color transitions. |
| `characters` | `string` | `"ABCDEFGHIJKLMNOPQRSTUVWXYZ!@#$&*()-_+=/[]{};:<>.,0123456789"` | Set of characters to glitch. |

You can edit these props directly in the `index.html` file (look for the `<GlitchCanvas>` call inside `ed()`).

## 🛠️ Technologies

- [React 19](https://react.dev/)
- [React DOM](https://react.dev/)
- HTML5 Canvas API
- Tailwind CSS (used via inline styles and utility classes)

All dependencies are inlined within the HTML file—no external CDN requests.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Enjoy the glitch!**
