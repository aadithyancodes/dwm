
# dwm — dynamic window manager

A fast, minimalist, and dynamic tiling window manager for X.

---

## ✨ Features

- Simple and ultra-lightweight (~2K SLOC)
- Dynamic tiling layouts
- Highly configurable at compile-time
- Status bar integration

---

## ⚙ Requirements

- Xlib development headers

---

## 📦 Installation

```bash
git clone https://git.suckless.org/dwm
cd dwm
vim config.mk    # adjust paths if needed
sudo make clean install
````

---

## 🚀 Getting Started

1. Add to `.xinitrc`:

   ```bash
   exec dwm
   ```

2. Optional: connect to a specific display

   ```bash
   DISPLAY=foo.bar:1 exec dwm
   ```

3. Show date and uptime in the status bar:

   ```bash
   while xsetroot -name "$(date) $(uptime | sed 's/.*,//')"; do
       sleep 1
   done &
   exec dwm
   ```

---

## 🔧 Configuration

dwm is configured by editing `config.h` and recompiling:

```bash
vim config.def.h    # modify defaults
cp config.def.h config.h
sudo make clean install
```

---

## 📄 Documentation

* [Official site](https://dwm.suckless.org/)
* [Manual](https://dwm.suckless.org/manual/)
* [FAQ](https://dwm.suckless.org/faq/)


