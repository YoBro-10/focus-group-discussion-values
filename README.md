# Culture Values Alignment Boards

A real-time, collaborative tool designed for focus group discussions to identify and compare current vs. preferred organizational culture. Built with **HTML5**, **Tailwind CSS**, and **Firebase Realtime Database**.

## 🚀 Live Demo
* **Phase 1: Current Culture Values** -> `index.html`
* **Phase 2: Preferred Culture Values** -> `preferred.html`

## 🛠 Features
- **Real-time Collaboration:** Multiple participants can drag/click words into culture baskets simultaneously.
- **Dual-Board Architecture:** Separate data paths for "How we are now" vs "How we want to be."
- **Mobile Friendly:** Supports both Drag-and-Drop and Click-to-Select for touch devices.
- **Admin Suite:** Facilitators can export results to CSV and reset boards via URL parameters.

## 📋 How to Use

### For Participants
1. Open the provided link (e.g., `index.html`).
2. Select a word from the **Available Pool**.
3. Click on the target **Culture Basket** to place it.
4. Use the top navigation bar to switch between "Current" and "Preferred" boards as directed by the facilitator.

## 🏗 Setup & Deployment

1. **Firebase:** - Create a Firebase project.
   - Enable **Anonymous Authentication**.
   - Enable **Realtime Database** and set rules to allow read/write.
   - Update the `firebaseConfig` object in both HTML files with your API keys.

2. **GitHub Pages:**
   - Upload `index.html` and `preferred.html` to a GitHub repository.
   - Go to **Settings > Pages** and enable hosting from the `main` branch.

## 📂 Data Structure
The app uses two distinct nodes in the Firebase Realtime Database:
- `baskets_current/`: Stores selections for the Current Culture board.
- `baskets_preferred/`: Stores selections for the Preferred Culture board.

---
*Developed for Focus Group Discussions & Cultural Transformation Workshops.*
