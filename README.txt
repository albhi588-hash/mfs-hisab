MFS Hisab Cloud - Firebase version

1. Upload the contents of this ZIP to your Render Static Site.
2. Firebase Authentication -> Sign-in method: Email/Password must be Enabled.
3. Firebase Firestore -> Rules: copy firestore.rules and Publish.
4. Open your Render URL and create the Owner account.
5. If an old white page is cached, press Ctrl+F5.

This version fixes the "save is not defined" browser error by using explicit DOM element lookup instead of relying on element IDs becoming JavaScript globals.
