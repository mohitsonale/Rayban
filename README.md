# 🕶️ Animated Ray-Ban Landing Page

A stylish, interactive landing page inspired by Ray-Ban’s bold branding — featuring advanced gooey background effects and animated hero text, built with **HTML**, **CSS**, **JavaScript**, **GSAP**, **Three.js**, and **Shery.js**.

---

## ✨ Features

- **Gooey Image Distortion**  
  The background uses `Shery.imageEffect()` to create a fluid, interactive gooey distortion that reacts to mouse movement and scroll.
  
- **Animated Hero Text**  
  Hero section text rotates on click — each line smoothly slides up using **GSAP** easing and timeline logic.
  
- **Clean, Modern Layout**  
  Minimal navbar, hero left and right split, full-screen visuals.
  
- **Responsive & Lightweight**  
  No frameworks or build tools — pure HTML, CSS, and JS with CDNs.

---

## 🚀 Live Preview

Github link:-https://github.com/mohitsonale/Rayban.git

---

## 🧩 Tech Stack

- **HTML5**
- **CSS3**
- **JavaScript (ES6)**
- **GSAP** — for robust animations and easing.
- **Three.js** — for potential 3D or canvas effects.
- **Shery.js** — for advanced web motion and gooey effects.

---


🪄 Hero Text Animation

var elems = document.querySelectorAll(".elem");
elems.forEach(function (elem) {
  var h1s = elem.querySelectorAll("h1");
  var index = 0;
  var animating = false;

  document.querySelector("#main").addEventListener("click", function () {
    if (!animating) {
      animating = true;
      gsap.to(h1s[index], {
        top: "-=100%",
        ease: Expo.easeInOut,
        duration: 1,
        onComplete: function () {
          gsap.set(this._targets[0], { top: "100" });
          animating = false;
        },
      });
      index = index === h1s.length - 1 ? 0 : index + 1;
      gsap.to(h1s[index], {
        top: "-=100%",
        ease: Expo.easeInOut,
        duration: 1,
      });
    }
  });
});

=>When you click anywhere in #main, the current line slides up and the next slides in. This creates an engaging, looped hero text carousel.

📂 Folder Structure

 1. index.html
 2. style.css
 3. script.js
 4. raybanlogo.png
 5. IMG_7564.JPG
 6. IMG_7565.JPG
 7. IMG_7566.JPG
 8. IMG_7567.JPG
 9. IMG_7568.JPG

⚡ Getting Started
1️⃣ Clone this repository:
https://github.com/mohitsonale/Rayban.git

2️⃣ Open the folder:

cd Rayban

📸 Screenshots
https://github.com/mohitsonale/Rayban/tree/9219c9d113c9bf46767e4ca434d2393a564f3ca8/images

OUTPUT:-
https://github.com/user-attachments/assets/3216c258-6015-4324-8d4d-c49353e72088

🪪 License
This project is open-source under the MIT License.

✍️ Author
Mohit Tushar Sonale
GitHub:-mohitsonale
LinkedIn:-Mohit Sonale

📣 Show Some ❤️
If you like this project:

⭐ Star it on GitHub

-Fork it and create your own version

-Tag me if you build on top of it!



