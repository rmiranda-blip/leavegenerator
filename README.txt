CDA HR System - Ready to use
---------------------------

How to use:
1. Unzip the folder "hr-firebase-site.zip".
2. Open index.html in your browser.
3. Login using default credentials:
   Username: admin
   Password: cda123
4. On the dashboard you can add employees, upload a photo (preview shown), edit, and delete.
5. Data syncs in real-time with your Firebase Realtime Database under "employees/".
   Make sure your Realtime Database rules allow writes during testing:
   {
     "rules": {
       ".read": true,
       ".write": true
     }
   }

Notes:
- The firebase config is already embedded in scripts/firebase-app.js using the config you provided.
- Photos are stored as base64 Data URLs inside the database (small images recommended).
- For production, consider using Firebase Storage for images and stricter DB rules.

