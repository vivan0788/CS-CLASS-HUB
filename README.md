🎓 CR Class Hub — 6 Subjects Engineering Resource Portal

A centralized, responsive, and lightweight web portal designed for Engineering Class Representatives (CR) to distribute lecture notes, assignment sheets, interactive tutorials, and high-resolution lab circuit setups to students without cluttering chat groups.

🚀 Live Demo & Screenshots

Single-File Architecture: Built entirely in a self-contained index.html file using modern HTML5, Tailwind CSS, and ES Module JavaScript.

Dual Role System: Seamless switching between Student Mode (read-only, bookmarking, downloads) and CR Admin Mode (password-protected resource uploads, edits, and live announcements).

📚 6 Core Engineering Subjects Supported

The portal is tailored with dedicated filters, badges, and counters for the following 6 core subjects:

Mathematics (Calculus, differential equations, tutorials, problem sets)

Applied Chemistry (Lab titrations, experiments, viva guides, water hardness calculations)

Electronics Engineering (CRO waveforms, breadboard rectifier setups, 74-series TTL logic IC pinouts)

Programming Language (C / Data Structures, code repositories, dynamic memory allocation)

Professional Communication (Technical report formats, resume writing, IEEE citation guidelines)

Artificial Learning and Machine Learning (Python notebooks, Jupyter Colab links, machine learning algorithms)

✨ Key Features

👨‍🎓 For Students

Instant Search & Multi-Filter: Search materials by faculty name, topic keywords, or experiment title. Filter easily by subject or resource category (Lab Images, Notes, Assignments, Tutorials).

Interactive Lab Lightbox: Click on any lab apparatus or circuit setup photo to zoom in, zoom out, reset, and pan/drag across the breadboard or IC pin connections.

Assignment Countdown Tracking: Automatic dynamic badges indicating status (Due in X days, Due Tomorrow, Due Today!, or Overdue).

CR Pro-Tips: Notice callouts containing teacher-specific instructions (e.g., compulsory questions, lab manual guidelines, or graphing tips).

Revision Bookmarks: Save important notes and formulas directly to browser storage for last-minute exam prep.

Dark / Light Mode: Built-in theme switcher with preference memory.

👑 For Class Representative (CR Admin Mode)

PIN/Password Verification Modal: Secure access control with a show/hide password toggle.

Add / Edit / Delete Materials: Modal form to upload new links (Google Drive, Cloudinary, PDFs, or Image URLs).

Live Class Notice Broadcaster: Pin urgent alerts directly to the top banner (e.g., room change, lab coat reminder, submission deadline extension).

Real-Time Cloud Sync: Syncs data automatically across all classmates using Firebase Firestore, with automatic LocalStorage fallback when offline.

🛠️ Tech Stack

Frontend: HTML5, CSS3, JavaScript (ES6 Modules)

Styling: Tailwind CSS CDN

Icons: Lucide Icons

Database & Auth: Google Firebase Firestore + Firebase Anonymous Auth

Storage Compatibility: Compatible with Google Drive links, GitHub repositories, and image hosting URLs.

🔐 Default CR Credentials

Role

Default Password

Access

Class Representative

Avinash0788

Full Admin (Upload, Edit, Delete, Post Notice)

Students

None required

Read-only browsing, downloads, and bookmarks

Note to CR: To change your password, search for crPassword: '*******0788' inside the <script> tag in index.html and update it with your desired string.

⚡ Quick Start / Local Setup

No npm install or local server build steps are required.

Clone or Download the repository:

git clone https://github.com/your-username/cr-student-portal.git
cd cr-student-portal


Open the project:

Simply double-click index.html to open it in any web browser (Chrome, Edge, Firefox, Safari).

Alternatively, open it with VS Code's Live Server extension.

🌐 Free Hosting Guide

You can host this website online for free so your entire class can access it via a link:

Option 1: GitHub Pages (Recommended)

Create a new repository on GitHub (e.g., cr-class-hub).

Push your index.html and README.md to the main branch.

Go to Repository Settings > Pages.

Under Branch, select main and root /, then click Save.

Your website will be live in 1-2 minutes at:
https://vivan0788.github.io/cs-class-hub/

Option 2: Netlify / Vercel (Drag & Drop)

Go to Netlify Drop.

Drag and drop the folder containing your index.html.

Netlify will instantly provide you with a live URL (e.g., https://cr-class-hub.netlify.app).

☁️ Setting Up Google Firebase (Optional)

If you wish to synchronize database entries across multiple devices in real-time:

Go to the Firebase Console and create a free project.

Enable Firestore Database in test mode.

Enable Authentication > Sign-in method > enable Anonymous.

In your Firebase Project Settings, copy the firebaseConfig object.

In index.html, pass your configuration into __firebase_config or replace setupFirebase() with your config keys.

If no Firebase configuration is supplied, the portal will automatically use browser localStorage with pre-loaded mock data.

📄 License

Distributed under the MIT License. Feel free to modify and adapt this template for your college or department batch!
