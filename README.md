# 🇮🇩 Merah Putih Duotone

A simple web tool that converts any image into a **red–white duotone**, inspired by the Indonesian flag.
Built with **HTML5 Canvas** + **JavaScript**, styled with modern CSS.

---

## ✨ Features

* 🎨 **Duotone Effect**
  Converts your image into a red (shadows) + white (highlights) duotone style.

* 📂 **Multiple Upload Options**

  * Drag & drop
  * File picker
  * Paste directly from clipboard (Ctrl/⌘ + V)

* 👀 **Preview & Compare**
  Toggle between original and processed image with **View Original**.

* 💾 **Download**
  Save your duotone image as PNG (`filename-edit.png`).

---

## 📸 Demo

👉 Try it live here: [Merah Putih Filter Demo](https://merah-putih-filter.vercel.app/)

1. Choose or drop an image.
2. See the **Merah Putih duotone preview** instantly.
3. Compare with the original if you want.
4. Download your processed image.

---

## 🗂 Project Structure

```
.
├── index.html       # Main app logic and UI
├── css/
│   └── style.css    # Styles (dark-themed, Jakarta Sans font)
```

---

## 🚀 Getting Started

1. Clone or download this repo.
2. Open `index.html` in your browser.
3. Drop an image and enjoy the duotone effect!

No build tools or frameworks required — **just pure HTML, CSS, and JS**.

---

## ⚙️ Tech Stack

* HTML5 `<canvas>` for pixel manipulation.
* Vanilla JavaScript (no dependencies).
* Modern CSS with custom properties for easy theming.

---

## 🖌 How It Works

* Each pixel is read and converted to **luminance**:

  ```js
  t = (0.299 * R + 0.587 * G + 0.114 * B) / 255;
  ```
* Luminance `t` is used to interpolate between:

  * **Red** `(255, 0, 0)` → shadows
  * **White** `(255, 255, 255)` → highlights
* The processed pixels are drawn back to the canvas.

---

## 📜 License

MIT License — free to use, modify, and share.
