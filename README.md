🎬 Modular Media Streaming Suite

A refactored and extensible media player built with JavaScript (ES6), applying structural design patterns for modularity, runtime flexibility, and plugin-driven enhancement.

🧩 Features

Multiple media sources: Local files, HLS streams, and Remote API sources

Composite playlists: Recursive folder + file playlists from index.json

Plugin system: Subtitles, Equalizer, and Watermarking toggleable at runtime

Renderer strategies: Switch between Hardware and Software renderers dynamically

Remote proxy & caching: Service Worker caches video streams for offline or faster playback

⚙️ How to Run the Project
1. Clone the Repository
git clone https://github.com/joshuaserrano224/Laboratory2.git
cd Laboratory2

2. Open in VS Code

Make sure you have the Live Server extension installed.

3. Start the Demo

Right-click index.html → “Open with Live Server”

This will launch:

http://127.0.0.1:5500/index.html


🧪 How to Test
▶️ Demo Interaction

Use the renderer dropdown to switch between Hardware and Software — overlay text will confirm.

Click “Load Local File”, “HLS Stream”, or “Remote API” to play different sources.

Toggle Subtitles, Equalizer, or Watermark plugins.

Browse your playlist panel — supports nested folders.


🧠 Design Patterns Used

Composite Pattern: Recursive playlists (playlist/index.json + nested folders)

Strategy Pattern: Runtime switching between renderers (hardware/software)

Decorator Pattern: Feature plugins dynamically add functionality

Facade Pattern: MediaFacade provides unified control for playback

Proxy Pattern: Service Worker handles remote caching
