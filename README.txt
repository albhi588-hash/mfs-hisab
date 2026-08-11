MFS HISAB — RENDER ROOT DEPLOYMENT

GitHub structure:
index.html
config.js
render.yaml
firebase/firestore.rules

Render:
Build Command: leave empty
Publish Directory: .

Firebase:
1. Authentication > Sign-in method > Email/Password = ON
2. Firestore Database = Create database
3. Paste firebase/firestore.rules into Firestore Rules and Publish
4. public/config.js is now root config.js. Replace its values if needed.

The Firebase Web config is already filled with the supplied project config.
