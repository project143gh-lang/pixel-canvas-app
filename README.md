# Pixel Canvas App

A creative pixel canvas web application. Draw, create, and express yourself with pixels on a grid canvas!

## 📸 Screenshot

![Pixel Canvas App Repository](./pixel-canvas-app.png)

**Start drawing:** Open `index.html` in any modern browser or run `npm start` after installing dependencies.

## Features

### 🎨 Drawing Tools
- **Pixel brush**: Paint individual pixels or fill areas
- **Color palette**: 21+ pre-configured colors with custom input
- **Eraser**: Remove pixels or clear areas
- **Fill bucket**: Flood fill tool for large areas

### 📐 Canvas Settings
- **Grid size**: Adjustable from 10x10 to 100x100 pixels
- **Zoom level**: Scale the canvas up to 5x
- **Undo/Redo**: Step back and forth through your changes
- **Clear canvas**: One-click complete reset

### 💾 Save & Share
- **Save locally**: Download your artwork as PNG
- **Load saved**: Reopen previously saved creations
- **Copy to clipboard**: Copy image data
- **Reset**: Start fresh anytime

### 🎯 User Experience
- Smooth drawing with keyboard shortcuts
- Responsive canvas resizing
- Color history panel
- Tool toggle hotkeys

## 🚀 Quick Start

### With Dependencies (Full Features):
```bash
# 1. Install dependencies
npm install

# 2. Run the application
npm start

# 3. Open in browser
# Visit: http://localhost:3000
```

### Without Dependencies (Basic):
```bash
# Just open index.html in any browser
open index.html
```

## 🛠️ Project Structure

```
mee.ai/
├── index.html          # Main HTML canvas application
├── package.json        # Node.js dependencies and scripts
├── server.js           # Node.js HTTP server with WebSocket support
├── PixelCanvas.js      # Core canvas logic and drawing algorithms
├── sidebar.html        # Collapsible tool palette UI
├── structure/          # Configuration and assets
│   └── config.json     # Canvas settings and defaults
├── PixelCanvas.js      # Rendering engine
├── styles.css          # Visual styling and color palettes
└── script.js           # Application state and event handling
```

## 📁 Subdirectory Details

### `structure/`
- `config.json`: Canvas dimensions, color palette, settings
- Additional structure files for layout and assets

### `PixelCanvas.js`
- Core rendering engine
- Pixel manipulation algorithms
- Undo/redo history manager
- Save/Load functionality

### `script.js`
- Application state management
- Tool selection and switching
- Keyboard shortcuts handler
- UI update logic

### `sidebar.html`
- Collapsible tool palette
- Color selector grid
- Brush size control
- Undo/redo buttons

## 💾 File Formats

### Save Format (JSON)
```json
{
  "width": 64,
  "height": 64,
  "pixels": [
    ["color1", "color1", "clear", ...],
    ["clear", "color2", "color2", ...],
    ...
  ]
}
```

### Image Export
- PNG format via canvas `toDataURL()`
- Downloadable from the UI

## 🎯 Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl + Z` | Undo last action |
| `Ctrl + Y` | Redo last action |
| `Ctrl + S` | Save current drawing |
| `Ctrl + Shift + Z` | Redo |
| `Backspace` | Clear canvas |
| `1-9` | Quick color selection |
| `Space` | Toggle eraser mode |
| `Arrow keys` | Nudge selected pixel |

## 📜 License

MIT

---

**K.bhalavardt, MIT Student**