# 🎙️ Voice Presentation Controller

A modern, browser-based **voice-controlled presentation viewer** that lets you open PDF and PowerPoint presentations and navigate through slides hands-free.

Simply say **"Next slide"** or **"Previous slide"** to control your presentation without reaching for the keyboard or mouse.

Built with a clean, minimalist dark interface and designed to work entirely in the browser.

## ✨ Features

### 🎙️ Voice Control

* Hands-free presentation navigation
* **"Next slide"** → Move to the next slide
* **"Previous slide"** → Move to the previous slide
* Live voice recognition status
* Voice control can be enabled or disabled from Settings

### 📑 Presentation Support

* Open **PDF** presentations
* Open **PowerPoint `.pptx`** presentations
* Drag & drop presentations directly into the application
* Resume presentations from the last viewed slide

### 🎛️ Presentation Controls

* Next / Previous slide navigation
* Clickable presentation progress bar
* Zoom in / Zoom out
* Reset zoom
* Fullscreen mode
* Keyboard shortcuts

### ⌨️ Keyboard Shortcuts

| Key       | Action            |
| --------- | ----------------- |
| `→`       | Next slide        |
| `←`       | Previous slide    |
| `+` / `=` | Zoom in           |
| `-`       | Zoom out          |
| `0`       | Reset zoom        |
| `F`       | Toggle fullscreen |
| `Esc`     | Exit fullscreen   |

### 🕘 Presentation History

The application remembers recently opened presentations and the last slide you viewed.

History is stored locally in the browser using `localStorage`.

### ⚙️ Settings

The Settings panel allows you to configure:

* Voice control
* Default zoom level
* Fullscreen when opening a presentation
* Microphone selection

## 🖥️ Interface

The application uses a minimalist dark interface focused on keeping presentation controls simple and distraction-free.

**Main interface includes:**

* Presentation library
* Voice status
* Quick voice commands
* Keyboard shortcuts
* Presentation progress
* Zoom controls
* Fullscreen controls
* Settings
* Presentation history

## 🛠️ Tech Stack

* **HTML5**
* **CSS3**
* **JavaScript (ES Modules)**
* **Web Speech API**
* **PDF.js**
* **PPTX Browser**
* **LocalStorage API**

### Libraries

* `pdf.js` for rendering PDF presentations
* `pptx-browser` for rendering PowerPoint presentations

## 📁 Project Structure

```text
voice-presentation-controller/
│
├── css/
│   └── main.css
│
├── js/
│   ├── adapters/
│   │   ├── platform/
│   │   │   └── browser-platform.js
│   │   ├── storage/
│   │   │   └── local-storage-adapter.js
│   │   └── voice/
│   │       └── web-speech-adapter.js
│   │
│   ├── core/
│   │   ├── command-parser.js
│   │   ├── history-manager.js
│   │   ├── presentation-controller.js
│   │   ├── presentation-state.js
│   │   └── settings-manager.js
│   │
│   ├── viewer/
│   │   └── presentation-viewer.js
│   │
│   ├── app.js
│   └── config.js
│
├── vendor/
│   └── pdfjs/
│
├── index.html
├── package.json
├── package-lock.json
├── LICENSE
└── .gitignore
```

## 🚀 Getting Started

### Prerequisites

Make sure you have:

* Node.js
* npm
* A modern browser with JavaScript enabled

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/voice-presentation-controller.git
```

### 2. Open the project

```bash
cd voice-presentation-controller
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the local server

```bash
npm start
```

The application will start using a local development server.

Open the displayed local URL in your browser.

## 🎤 Using Voice Commands

1. Open the application.
2. Enable **Voice Control**.
3. Open a PDF or PowerPoint presentation.
4. Start presenting.
5. Use voice commands to navigate.

### Example

```text
"Next slide"
       ↓
Next slide
```

```text
"Previous slide"
       ↓
Previous slide
```

The application also provides keyboard controls if voice recognition is unavailable.

## 🔐 Privacy

Presentation files are processed locally in the browser and are not uploaded by the application.

The application also stores presentation history and settings locally using browser storage.

Voice recognition uses the browser's built-in speech recognition capability. Depending on the browser, speech processing may be handled by the browser vendor's speech recognition service.

## 🌐 Browser Compatibility

Voice recognition depends on browser support for the **Web Speech API**.

If voice recognition is unavailable, presentations can still be controlled using keyboard and on-screen controls.

For the best experience, use a modern Chromium-based browser with speech recognition support.

## 🔮 Future Improvements

* [ ] Standalone Windows `.exe`
* [ ] Improved voice command customization
* [ ] More presentation commands
* [ ] Start / stop presentation mode
* [ ] Voice command for fullscreen
* [ ] Voice command for zoom
* [ ] Presentation timer
* [ ] Better microphone management
* [ ] Custom themes
* [ ] More presentation formats
* [ ] Installer for Windows

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome.

If you find a bug or have an idea for a new feature, feel free to open an issue or submit a pull request.

## 📄 License

This project is licensed under the **MIT License**.

See the [`LICENSE`](LICENSE) file for details.

---

⭐ If you find this project useful, consider giving it a star!
