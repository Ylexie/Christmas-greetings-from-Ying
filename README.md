# 🎄 Interactive 3D Particle Christmas Card – Greetings From Ying

A festive web app featuring a 3D particle-based Christmas tree that reacts to your hand movements using MediaPipe Hands and Three.js.

Make different gestures to spread and gather the particles, and show an **OK** sign to trigger a full-screen particle explosion and reveal a Santa-themed greeting card with energetic English Christmas wishes.

Live demo (GitHub Pages):

👉 https://ylexie.github.io/Christmas-greetings-from-Ying/ChristmaswishesFromYing.html  
(or, if you rename the file to `index.html`:  
👉 `https://ylexie.github.io/Christmas-greetings-from-Ying/`)

---

## ✨ Features

- **3D particle Christmas tree**
  - Built with Three.js point clouds.
  - Colorful lights and decorations.
  - Starry particle background with subtle rotation and twinkling.

- **Hand gesture interaction (MediaPipe Hands)**
  - Real-time tracking of one hand from the webcam.
  - Hand movement affects the tree’s rotation, position, and scale.
  - Different gestures map to different behaviors:
    - 👊 **Fist** – particles gather and compress into a tighter tree shape.
    - 🖐 **Open hand** – particles gently spread out around the tree.
    - 👌 **OK gesture** – triggers the “magic moment”:
      - The tree explodes into a dispersed particle cloud.
      - Santa-like particle figures appear.
      - A greeting card with a random English Christmas wish is shown.

- **Santa particle figures & sleigh**
  - Two Santa silhouettes made of particles appear on each side after the OK gesture.
  - A separate particle cluster orbits like Santa’s sleigh, gently bobbing up and down.

- **Dynamic Christmas background music (Tone.js)**
  - Starts after the user clicks the “Enable Camera / Start Tracking (Play Music)” button.
  - Simple synthesized melody inspired by classic Christmas tunes.

- **Random English greetings**
  - Each OK gesture reveals one random message from a list of upbeat, fun English Christmas wishes.
  - The greeting is displayed in a centered card-style overlay, perfect for screenshots or sharing.

---

## 🕹 How to Use

1. Open the web app in a browser and click the top button:

   **“Enable Camera / Start Tracking (Play Music)”**

   The browser will ask for permission to use the camera.  
   ➜ Click **Allow**.

2. Put your hand in front of the camera (ideally in the center region of the preview):

   - **Open hand**
     - Tree particles spread out slightly.
     - Status text shows:  
       > Open hand detected! Particles dispersing (Spreading)...

   - **Fist**
     - Particles gather into a denser tree.
     - Status text shows:  
       > Fist detected! Particles gathering (Compressing)...

   - **OK gesture** (thumb and index finger forming a circle)
     - Hold the OK gesture for ~0.4 seconds.
     - The tree explodes into a dispersed particle field.
     - Santa particle figures become visible.
     - A random Christmas greeting appears in the center.
     - Status text shows:  
       > Christmas blessing delivered!

3. Click the **“Reset Scene”** button at the bottom to:
   - Rebuild the tree.
   - Hide Santa and the card.
   - Get a new random greeting for the next OK gesture.

---

## 🌐 Browser & Device Tips

- Recommended browsers:
  - **Desktop**: Chrome / Edge / Firefox (with WebGL and `getUserMedia` support).
  - **Mobile**:
    - Android: Chrome  
    - iOS: Safari (do *not* open inside WeChat’s built-in browser if possible).

- Make sure to:
  - Allow camera access when prompted.
  - Use good lighting so your hand is clearly visible.
  - Keep your hand reasonably close so it occupies a noticeable part of the video.

---

## 🛠 Tech Stack

- **HTML + CSS + Vanilla JavaScript**
- **Three.js r128** – 3D scene, particles, tree, stars, Santa figures, sleigh.
- **MediaPipe Hands @0.4 (CDN)** – hand landmark detection and gesture logic.
- **Tone.js** – simple synthesized Christmas background music.
- No bundlers, no frameworks – everything lives inside a single HTML file, ideal as a demo or personal greeting card.

---

