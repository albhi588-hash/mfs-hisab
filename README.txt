MFS HISAB — RENDER + FIREBASE
==============================

এই project Render Static Site হিসেবে deploy করার জন্য প্রস্তুত।

FOLDER
------
public/
  index.html
  config.js
firebase/
  firestore.rules
render.yaml
README.txt

STEP 1 — Firebase
-----------------
1. Firebase Console-এ project তৈরি করো।
2. Authentication > Sign-in method > Email/Password ON করো।
3. Firestore Database তৈরি করো।
4. Project settings > Your apps > Web app > Register app।
5. Firebase যে firebaseConfig দেবে, সেটা public/config.js-এর values-এ বসাও।

STEP 2 — Firestore Rules
------------------------
firebase/firestore.rules-এর rules Firebase Console > Firestore Database > Rules-এ paste করে Publish করো।

STEP 3 — GitHub
---------------
1. GitHub-এ নতুন repository বানাও, যেমন: mfs-hisab
2. এই project-এর public folder, render.yaml, firebase folder, README.txt repository-তে upload করো।
3. config.js-এ Firebase config বসিয়ে commit করো।

STEP 4 — Render
---------------
1. Render Dashboard খুলে New > Static Site নির্বাচন করো।
2. GitHub connect করো এবং mfs-hisab repository নির্বাচন করো।
3. Branch: main
4. Build Command: খালি রাখো
5. Publish Directory: public
6. Create Static Site / Deploy করো।

Render deploy শেষ হলে তোমাকে একটি *.onrender.com address দেবে।

STEP 5 — Test
-------------
1. Render URL খুলে Register দিয়ে Owner account তৈরি করো।
2. Login করো।
3. DSO যোগ করো।
4. Customer যোগ/বাকি entry দাও।
5. Transaction entry দাও।

IMPORTANT
---------
এটি Firebase client SDK ব্যবহার করে। Firebase Web config সাধারণত frontend-এ থাকে; database নিরাপত্তা Firestore Rules দিয়ে করতে হয়।

বর্তমান starter version-এ account-level isolation আছে: প্রতিটি login নিজের data দেখে।
Production DSO system বানানোর আগে Owner/DSO role, DSO-specific access, transaction approval, audit log এবং dispute flow যোগ করা উচিত।

Render static site-এ server-side code লাগে না। GitHub branch-এ push করলে Render automatic redeploy করতে পারে।
