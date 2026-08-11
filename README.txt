MFS HISAB CLOUD — RENDER SETUP

1) ZIP extract করুন।
2) GitHub repository-তে index.html upload/replace করুন।
3) Render Static Site → আপনার GitHub repo।
4) Build Command: খালি রাখুন।
5) Publish Directory: .
6) Save/Deploy করুন।

Firebase:
- Project: dsohisab
- Email/Password Authentication enabled থাকতে হবে।
- Firestore Database তৈরি থাকতে হবে।
- আপনার দেওয়া Firebase Web config index.html-এ বসানো আছে।

প্রথম login:
- New account / Owner দিয়ে নিজের account বানান।
- তারপর Owner Dashboard থেকে DSO account তৈরি করুন।
- DSO তার email/password দিয়ে ফোনে একই Render link খুলে login করবে।

গুরুত্বপূর্ণ:
এটি একটি working MVP। বর্তমান Firestore rules logged-in users-এর access দেয়। Production ব্যবহারের আগে role-based security rules শক্ত করা উচিত।
