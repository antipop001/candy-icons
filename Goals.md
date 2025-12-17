# Candy-Neon

A personal fork of the KDE **Candy** icon theme with custom, SVG-first enhancements.

This fork follows upstream Candy conventions closely, including support for **Chrome PWA icon aliases**, so apps like Google Messages and WhatsApp automatically pick up themed icons without modifying `.desktop` files.

**Upstream project:**  
https://github.com/EliverLara/candy-icons

---

## 🎯 Goals

- Preserve full compatibility with upstream Candy
- Use **SVG-first** workflow for all new icons
- Add a clean, modern **Messages** icon
- Match Candy’s handling of **Chrome PWAs**
- Ensure perfect scaling from **16px → HiDPI**
- Make the theme portable across machines via Git

---

## 🎨 Design Philosophy

All new icons in this fork follow these rules:

- **Outline-only** (no fills)
- **Transparent background**
- **No blur, glow, particles, or filters**
- Rounded geometry
- Candy-style **gradient strokes**
- Simple paths for clean SVG rendering

---

## ✉️ Messages Icon

### Specification
- Canvas: `1024 × 1024`
- ViewBox: `0 0 1024 1024`
- Stroke-only SVG
- Rounded caps and joins
- Diagonal Candy-style gradient

### Gradient Stops
```
#2EE9FF
#4D7CFF
#7A4DFF
#C83CFF
#FF8A3C
```

---

## 🧩 Chrome PWA Support

Example Google Messages PWA desktop entry:
```
Icon=chrome-hpfldicfbfomlpcikngkocigghgafkph-Default
```

Icons provided:
```
scalable/apps/messages.svg
scalable/apps/chrome-hpfldicfbfomlpcikngkocigghgafkph-Default.svg
```

This mirrors upstream Candy’s handling of WhatsApp Web.

---

## 📦 Installation

```bash
git clone https://github.com/<your-username>/candy-icons ~/.local/share/icons/Candy-Neon
```

Enable in:
```
System Settings → Appearance → Icons
```

Reload Plasma if needed:
```bash
kquitapp5 plasmashell && plasmashell &
```

---

## 🛠 Development Status

### Completed
- Forked upstream Candy repository
- Cloned fork locally
- Designed and cleaned Messages SVG icon
- Verified Chrome PWA app IDs
- Matched upstream Candy PWA alias behavior

### In Progress
- Adding Messages SVG and Chrome alias to theme
- Committing changes to fork

---

## 📜 License

Same license as upstream Candy.  
All original artwork remains with their respective authors.

---

## 🙏 Credits

- Candy icon theme by **EliverLara**
- Fork and Messages icon by the author of this fork
