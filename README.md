# ✨ Serene Sleep - Mindful Green Noise Generator ✨

Welcome to Serene Sleep, a simple yet beautiful web application designed to help you relax, focus, or drift off to sleep with the soothing sounds of green noise. This app features multiple ambiance options and a calming, mindful visualization inspired by tranquility.


## 📜 Overview

In today's busy world, finding moments of peace can be challenging. Background noise, stress, and racing thoughts can make it hard to unwind or fall asleep. Serene Sleep aims to provide a digital sanctuary by generating customizable green noise – a specific frequency spectrum often compared to natural sounds like waterfalls or deep forests – known for its ability to mask distracting sounds and promote relaxation.

This application combines high-quality audio generation with a minimalist, aesthetically pleasing interface and a slow, meditative visual element, creating a holistic experience for mindfulness and rest.

## 🚀 Live Demo

Experience Serene Sleep directly in your browser:

**[➡️ Launch Serene Sleep Live Demo](https://noise.abhiramnj.com)**


## 🌟 Features

*   **Multiple Green Noise Ambiences:** Choose from several carefully crafted sound profiles:
    *   🌳 Forest Stream
    *   🌊 Distant Fall
    *   🌧️ Gentle Rain
    *   🍃 Rustling Trees
    *   🏖️ Calm Waves
    *   🌌 Deep Space (Ambient)
*   **Mindful Visualization:** A calming, abstract visualizer featuring:
    *   A gently pulsing "breathing" circle.
    *   Slowly drifting particles.
    *   Smooth color transitions that adapt to the selected ambiance.
*   **Preset Timers:** Set the noise to automatically fade out and stop after:
    *   15 minutes
    *   30 minutes
    *   90 minutes
    *   3 hours
*   **Volume Control:** Adjust the sound level to your preference.
*   **Play/Stop Controls:** Simple and clear playback management.
*   **Ambiance Autoplay:** Selecting a new ambiance automatically starts playback.
*   **Audio Fade-Out:** Timer expiration triggers a smooth volume fade before stopping.
*   **Responsive Design:** Adapts gracefully to desktops, tablets, and mobile devices.
*   **Single-File Application:** Easy to deploy and run – everything is in `index.html`.
*   **Modern Technologies:** Built with HTML5, CSS3 (Variables, Gradients, Grid/Flexbox), and Vanilla JavaScript (Web Audio API, Canvas API).

## 🕹️ How to Use

1.  **Open the App:** Launch the [Live Demo](#-live-demo) or open the `index.html` file locally.
2.  **(Optional) Choose Ambiance:** Select your preferred sound profile (it will start playing automatically).
3.  **Play/Stop:** Use the main "Play" or "Stop" buttons to control playback.
4.  **Adjust Volume:** Use the slider to set the desired sound level.
5.  **(Optional) Set Timer:** Click one of the timer buttons (15m, 30m, 90m, 3h) to have the sound automatically fade out and stop after that duration.
6.  **Relax:** Enjoy the calming sounds and visuals.

## 🛠️ Technology Stack

*   **HTML5:** Semantic structure for the application interface.
*   **CSS3:**
    *   Styling for layout, appearance, and theme.
    *   CSS Variables for dynamic theming (hue shifting).
    *   Gradients for backgrounds and visual effects.
    *   Flexbox & Grid for responsive layout.
    *   Transitions & Animations for smooth UI interactions.
*   **Vanilla JavaScript (ES6+):**
    *   **Web Audio API:** For generating, filtering (creating green noise variations), controlling volume, and playing audio.
    *   **Canvas API:** For rendering the dynamic, mindful visualization.
    *   **DOM Manipulation:** For handling user interactions, updating UI elements (buttons, timer display), and managing application state.
    *   **Event Handling:** Listening for clicks, slider changes, visibility changes, etc.

## 🏡 Running Locally

Since this is a single-file web application, running it locally is extremely simple:

1.  **Get the Code:**
    *   Clone the repository: `git clone https://github.com/twilighty-abhi/Green-noise-gen.git`
    *   OR Download the `index.html` file directly.
2.  **Open the File:** Navigate to the downloaded file/cloned directory and open the `index.html` file in your preferred modern web browser (like Chrome, Firefox, Safari, Edge).

That's it! The application should load and be ready to use.

## 📄 Code Structure (Single File: `index.html`)

The entire application is contained within the `index.html` file, organized as follows:

1.  **`<head>`:**
    *   Metadata (`charset`, `viewport`).
    *   Title.
    *   **`<style>` block:** Contains all the CSS rules defining the application's appearance, layout, responsiveness, and theme variables.
2.  **`<body>`:**
    *   **`<div class="container">`:** Main wrapper for the UI.
        *   `<h1>`: Application title.
        *   **`<div class="visualization">`:** Contains the `<canvas id="visualizer">` element where the JavaScript draws the animation.
        *   **`<div class="controls">`:** Contains all user interface elements:
            *   Ambiance selection buttons (`.sound-options`).
            *   Volume slider (`.volume-control`).
            *   Play/Stop buttons (`.main-buttons`).
            *   Timer preset buttons (`.timer-presets`).
            *   Timer display area (`.timer-display`).
            *   Footer text.
    *   **`<script>` block:** Contains all the JavaScript logic:
        *   Configuration constants.
        *   State variables (tracking playback, timer, audio nodes, etc.).
        *   DOM element references.
        *   Canvas setup and particle creation functions (`resizeCanvas`, `createParticles`).
        *   Web Audio API setup (`initAudio`, `createSoundNode`).
        *   Playback control functions (`playCurrentSound`, `stopPlayback`, `finalizeStop`).
        *   Visualization drawing logic (`startVisualization`, `stopVisualization`, `visualize`).
        *   Timer logic (`startTimer`, `clearTimer`, `updateTimerDisplay`).
        *   Event listener setup for all buttons, sliders, window resize, and visibility changes.
        *   Initial setup code that runs when the DOM is loaded.

## 💡 Potential Improvements & Customization

This project serves as a solid foundation. Here are some ideas for extending it:

*   **More Noise Types:** Add options for White Noise, Pink Noise, or Brown Noise with appropriate filtering.
*   **Advanced Ambiences:** Allow mixing sounds (e.g., Rain + Forest).
*   **Visualization Options:** Offer different visual styles or allow customization.
*   **User Preferences:** Use `localStorage` to save the user's last selected ambiance, volume level, or timer setting.
*   **Custom Timer:** Add an input field for setting a custom timer duration.
*   **Keyboard Shortcuts:** Implement shortcuts for Play/Stop and volume control.
*   **Progressive Web App (PWA):** Add a service worker and manifest for offline access and installability.
*   **Accessibility Enhancements:** Further review and improve ARIA attributes and keyboard navigation.

## 🙌 Contributing

Contributions are welcome! Whether it's reporting a bug, suggesting a feature, or submitting a code improvement, your help is appreciated.

1.  **Issues:** Feel free to open an issue to report bugs or discuss new features.
2.  **Pull Requests:**
    *   Fork the repository.
    *   Create a new branch for your feature or bugfix.
    *   Make your changes.
    *   Ensure the code works and is reasonably clean.
    *   Submit a Pull Request with a clear description of your changes.




Made with ❤️ Abhi and the calming power of green noise. Enjoy your moments of serenity!