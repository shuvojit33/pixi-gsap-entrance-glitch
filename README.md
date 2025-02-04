# 🚀 Entrance Animation & Glitch Effect with GSAP and PIXI.js

A dynamic animated **PIXI.js canvas** featuring a **smooth GSAP entrance animation** combined with a **random glitch effect**, built for an immersive **Awwwards-style** visual experience.

---

## 🎥 **Live Demo**
🔗 [View the Live Demo](https://dev.dascodes.com/project/pixi-gsap-entrance-glitch/)

---

## 📌 **Features**
- ✅ **Smooth GSAP Entrance Animation** – The canvas slides into view elegantly.
- ✅ **PIXI.js for WebGL rendering** – High-performance graphics.
- ✅ **Glitch Effect with PIXI Filters** – Adds a digital distortion effect.
- ✅ **Auto-resizing Canvas** – Supports dynamic width/height and Retina displays.
- ✅ **Customizable Settings** – Adjust animation, glitch intensity, and timing.

---

## 🚀 **Installation & Setup**
### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/shuvojit33/pixi-gsap-entrance-glitch.git
cd pixi-gsap-entrance-glitch
```

### **2️⃣ Open `index.html` Locally**
Simply open the `index.html` file in your browser.

OR start a simple local server:
```sh
npx serve .
```

### **3️⃣ View in Browser**
Go to `http://localhost:3000` or your local server URL.

---

## 🛠 **Customization**
### **Modify Canvas Size**
Update `.image-container` in your HTML:
```html
<div class="image-container" data-width="800" data-height="600">
    <canvas class="pixi"></canvas>
</div>
```

### **Change the Image**
Update `imgLink` in `js/demo.js`:
```javascript
const imgLink = "https://your-new-image-url.com";
```

### **Adjust Entrance Animation Timing**
Modify `runEntranceAnimation()` in `js/demo.js`:
```javascript
gsap.timeline()
    .set(canvas, { x: window.innerWidth + 50, scaleX: 1.5, scaleY: 0.8, opacity: 0.3 }, "begin+=1.05")
    .to(canvas, { duration: 0.2, ease: "expo.out", x: 0 }, "begin+=1.05")
    .to(canvas, { duration: 0.6, ease: "elastic.out(1, 0.7)", scaleX: 1, scaleY: 1, opacity: 1 }, "begin+=1.1");
```

---

## 📜 **Usage**
- 🎬 **Canvas smoothly enters the viewport** using GSAP animation.
- 🎭 **Glitch effect triggers randomly**, creating a digital distortion.
- 🖼️ **Works with any image or resolution** – fully responsive.

---

## 👨‍💻 **Contributing**
Pull requests are welcome! Please follow these steps:
1. **Fork the repository**
2. **Create a new branch** (`git checkout -b feature-branch`)
3. **Make your changes and commit** (`git commit -m "Added feature XYZ"`)
4. **Push to GitHub** (`git push origin feature-branch`)
5. **Open a Pull Request**

---

## 🔥 **Credits**
- 🎨 [PIXI.js](https://pixijs.com/) - High-performance WebGL rendering
- 🏆 [GSAP](https://greensock.com/gsap/) - Smooth animations
- 📷 Image Source: [Pixabay](https://pixabay.com/)




