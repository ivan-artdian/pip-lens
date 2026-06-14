# pip-lens

> A GNOME Shell extension for floating Picture-in-Picture overlays — pin any window or drag-select any screen region as a live, always-on-top thumbnail.

**pip-lens** is a fork of [WTMB (Window Thumbnails)](https://github.com/G-dH/window-thumbnails) by [G-dH](https://github.com/G-dH), extended with screen area/region capture — inspired by the Picture-in-Picture feature built into [elementary OS](https://elementary.io)'s [Gala](https://github.com/elementary/gala) window manager, which lets you pin either a window *or* a drag-selected area of the screen as a floating overlay.

---

## What's new in this fork

| Feature | Upstream (WTMB) | pip-lens |
|---|:---:|:---:|
| Window clone thumbnail | ✅ | ✅ |
| **Screen area / region capture** | ❌ | ✅ |
| Drag to select any screen region | ❌ | ✅ |
| Floating, always-on-top overlay | ✅ | ✅ |
| Drag to move thumbnail | ✅ | ✅ |
| Resize by scrolling | ✅ | ✅ |
| Minimize window to thumbnail | ✅ | ✅ |
| Full-size preview on hover | ✅ | ✅ |
| Custom scale, position, opacity | ✅ | ✅ |
| Custom keyboard shortcuts | ✅ | ✅ |
| Multi-monitor support | ✅ | ✅ |
| GNOME Shell 42–50 | ✅ | ✅ |

The key addition is **screen area capture**: instead of only being able to pin a whole window, you can now drag to select any rectangular region of the screen — a video player, a terminal output, a section of a document — and pin just that region as a live PIP thumbnail. This mirrors how elementary OS's built-in PIP works, where you can either click a window or drag across any part of it.

---

## Features

- Pin any **window** as a floating scaled-down clone
- **Drag-select any screen region** to create a region thumbnail
- Move thumbnails freely anywhere on screen via drag-and-drop
- Resize by scrolling the mouse wheel
- Minimize windows directly to their thumbnail
- Optional full-size preview on hover
- Optional hide on hover
- Custom default scale, position, opacity, and animation speed
- Fully customizable mouse and keyboard controls
- Unlimited thumbnails or limit to a single one
- Windows remember the position and size of their thumbnail
- Multi-monitor support

---

## Installation

### From GitHub

You may need to install `git`, `make`, `gettext`, and `glib2.0` first.

#### GNOME 45+

```bash
git clone https://github.com/ivan-artdian/pip-lens.git
cd pip-lens
make install
```

#### GNOME 42–44

```bash
git clone https://github.com/ivan-artdian/pip-lens.git
cd pip-lens
git checkout gnome-42-44
make install
```

### Enabling the extension

After installation, restart GNOME Shell:

- **X11:** Press `Alt` + `F2`, type `r`, press `Enter`
- **Wayland:** Log out and log back in

Then open the **Extensions** app, find *pip-lens*, and enable it.

---

## Usage

**Create a window thumbnail**
Click the extension icon or use the keyboard shortcut to select a window — it will appear as a floating PIP overlay.

**Create a screen region thumbnail**
Activate the extension, then drag across any area of the screen to pin just that region as a live thumbnail.

**Move / resize**
Drag the thumbnail to reposition it. Scroll the mouse wheel over it to resize.

---

## Credits

- [G-dH](https://github.com/G-dH) — original [WTMB (Window Thumbnails)](https://github.com/G-dH/window-thumbnails) extension
- [donadigo](https://github.com/donadigo) — original [`gala-pip-plugin`](https://github.com/donadigo/gala-pip-plugin), later merged into elementary OS's Gala, which inspired the area capture feature
- [elementary OS](https://elementary.io) — for building PIP (window + area selection) into their desktop as a first-class feature

---

## License

[GPL-3.0](LICENSE)
