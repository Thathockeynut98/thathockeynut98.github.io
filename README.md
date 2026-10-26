SyncSpace 🚀

Real-Time Collaborative Workspace & Ambient Space

SyncSpace is a lightweight, all-in-one collaborative environment designed for teams, friends, or long-distance partners to connect, collaborate, and hang out in real-time. It features real-time document editing, shared scratchpad notes, photo walls, YouTube watch parties, ambient audio, sleep/bedtime tracking, and a sketchpad.

✨ Features

📝 Synchronized Document Editor: Real-time collaborative document editing with auto-save across room participants.

📌 Quick Cards (Scratchpad): Post sticky notes and quick takeaways visible to everyone in the room.

🖼️ Shared Photo Wall: Pin photos and image links to build a shared memory board or collage.

🎵 Ambient Soundscapes: Built-in ambient background audio streams (Lo-Fi beats, Rain, Fireplace, Ocean Waves).

🎬 Watch Together Sync: Synchronize YouTube video playback for group viewing or listening parties.

🌙 Sleep Space & Wind-Down Zone: Bedtime tracking, gentle sleep sounds (Rain, Space, Fire, Waves), sleep timers, and night/morning messages.

🎨 Interactive Sketch Canvas: Draw, sketch, or brainstorm together on an interactive canvas.

😊 Mood & Distance Status: Share your current status and mood with room members.

💬 Live Chat & Active Presence: Real-time text messaging and live member presence updates.

🔗 Instant Room Sharing: Shareable room codes and direct links.

⚡ Standalone/Fallback Mode: Seamlessly falls back to an in-memory client state when offline or running without a Firebase config.

🛠️ Tech Stack

Frontend: Plain HTML5, Tailwind CSS (via CDN)

Icons: FontAwesome 6

Database / Backend: Firebase Firestore & Anonymous Authentication (JS SDK v11)

Audio & Media: HTML5 Web Audio API & YouTube Embedded IFrame API

🚀 Getting Started

Prerequisites

No complex build steps or node modules are required. The project runs directly in the browser.

Running Locally

Clone or download this repository:

git clone https://github.com/your-username/syncspace.git
cd syncspace


Open index.html in any modern web browser or use a local static web server like Live Server or python3 -m http.server 8000.

⚙️ Firebase Setup (Optional)

SyncSpace includes an automatic Standalone Mode that functions out-of-the-box without external server dependencies. To enable true multi-device persistence via Firebase:

Create a Firebase project at Firebase Console.

Enable Firestore Database and Anonymous Authentication.

Define your Firebase config in a script tag or environment variable before loading the app script:

<script>
  window.__firebase_config = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_PROJECT_ID.firebasestorage.app",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID"
  };
</script>


📄 License

This project is open-source and available under the MIT License.
