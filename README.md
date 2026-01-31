# 🧠 Sleep Serene - Focus & Sleep

A scientifically-backed sound generator featuring white, pink, brown noise, and binaural beats designed to enhance productivity and improve sleep quality.

## 🔬 Scientific Sound Types

### Productivity Mode
- **White Noise** - Equal power across all frequencies (20Hz-20kHz) for maximum masking
- **Pink Noise** - -3dB/octave rolloff, proven to improve work performance
- **Brown Noise** - -6dB/octave, deep rumbling for intense concentration
- **Focus Rain** - Optimized rainfall spectrum for blocking distractions
- **Beta Beats** (18Hz) - Binaural beats for active thinking and alertness
- **Gamma Beats** (40Hz) - Peak concentration and memory enhancement

### Sleep Mode
- **Pink Sleep** - Research shows enhanced deep sleep and memory consolidation
- **Brown Sleep** - Deeply calming low-frequency dominance
- **Ocean Waves** - Rhythmic pattern mimics breathing for relaxation
- **Night Rain** - Gentle, continuous masking optimized for rest
- **Delta Beats** (2Hz) - Deep sleep induction frequency
- **Theta Beats** (6Hz) - Promotes drowsiness and sleep onset

## 🌟 Features

- **Dual Mode System** - Switch between energizing productivity and calming sleep themes
- **Authentic Audio Generation** - Algorithmically precise noise using scientific algorithms
- **Binaural Beat Synthesis** - Stereo oscillator pairs for brainwave entrainment
- **Scientific Information** - Each sound includes frequency specs and research-backed benefits
- **Smart Timers** - Mode-specific presets (Pomodoro 25m for work, 8h for sleep cycles)
- **PWA Support** - Install as app, works offline with service worker
- **Keyboard Shortcuts** - Space (play/pause), M (mute), 1-6 (sounds)
- **Wake Lock** - Prevents screen dimming during sessions
- **Responsive Design** - Adapts to all screen sizes
- **Visual Feedback** - Animated visualizer responds to playback

## 🧬 The Science

### Noise Types
Colored noises are categorized by their power spectral density:
- **White Noise**: Flat power across all frequencies - excellent for masking
- **Pink Noise**: 1/f noise with equal energy per octave - more balanced than white
- **Brown Noise**: 1/f² noise following Brownian motion - deep, rumbling character

Research shows pink noise can enhance deep sleep (N3 stage), improve memory consolidation, and increase sleep spindle density. White noise has been shown to improve concentration in ADHD individuals and reduce sleep onset time.

### Binaural Beats
Created by playing slightly different frequencies to each ear:
- Brain perceives the mathematical difference as a "beat"
- May influence brainwave patterns through frequency following response
- **Delta (0.5-4Hz)**: Associated with deep, dreamless sleep
- **Theta (4-8Hz)**: Light sleep, meditation, drowsiness
- **Beta (13-30Hz)**: Active thinking, focus, alertness
- **Gamma (30-50Hz)**: Peak cognitive processing, memory

**Note**: Binaural beats require stereo headphones to work properly.

## 🕹️ How to Use

1. **Select Mode** - Choose between Focus (productivity) or Sleep mode
2. **Pick a Sound** - Browse scientifically-designed audio options
3. **Adjust Volume** - Recommended 40-60dB for sleep, 50-70dB for focus
4. **Set Timer** - Optional automatic shutoff (Pomodoro 25m, Sleep cycles 90m/8h)
5. **Read the Science** - Info panel explains each sound's benefits
6. **Use Headphones** - Required for binaural beats to be effective

### Keyboard Shortcuts
- `Space` - Play/Pause
- `M` - Mute/Unmute
- `1-6` - Select sounds 1 through 6

## 🛠️ Technology Stack

*   **HTML5** - Semantic structure with Web Audio API
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
