# 🥁 Drum Kit

> **Turn your keyboard into a drum set and make some noise! 🎵**

Drum Kit is an interactive **browser-based music experience** built using **HTML, CSS, and JavaScript**.

Instead of simply looking at a drum set, you get to **play it**. Click the drums with your mouse or use your keyboard to trigger different sounds and create your own beats.

---

## 🎵 What Can You Do?

### 🥁 Play Different Drums

The kit contains multiple drum sounds, including:

- 🪘 Tom 1
- 🪘 Tom 2
- 🪘 Tom 3
- 🪘 Tom 4
- 🥁 Snare
- 💥 Crash
- 🔊 Kick

Each drum is mapped to a specific keyboard key, allowing you to play the kit without touching your mouse. :contentReference[oaicite:1]{index=1}

---

## 🎮 Two Ways to Play

### 🖱️ Mouse

Click any drum button on the screen to trigger its corresponding sound.

### ⌨️ Keyboard

Use the assigned keyboard keys to play the drums:

| Key | Sound |
|---|---|
| `W` | Tom 1 |
| `A` | Tom 2 |
| `S` | Tom 3 |
| `D` | Tom 4 |
| `J` | Snare |
| `K` | Crash |
| `L` | Kick |

Keyboard events are captured using JavaScript's event handling system and mapped to individual audio files. :contentReference[oaicite:2]{index=2}

---

## ✨ Interactive Visual Feedback

Every time a drum is played, the corresponding button briefly changes its appearance.

This creates a visual response that makes the interaction feel more like a small browser game rather than a static webpage.

The animation is handled by adding and removing a `pressed` CSS class dynamically. :contentReference[oaicite:3]{index=3}

---

## 🧠 How It Works

The project follows a simple event-driven flow:

```text
          User Input
         /          \
      Mouse        Keyboard
        │              │
        └──────┬───────┘
               ↓
        JavaScript Event
               ↓
          Identify Key
               ↓
         Play Drum Sound
               ↓
       Trigger Animation
               ↓
        Visual Feedback
