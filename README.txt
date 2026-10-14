AWAIZ CHAT STARTER — READ FIRST

Includes email/password registration and login, registered-user list, real-time one-to-one text chat, Firestore rules, responsive UI, and Capacitor configuration.

1) Firebase setup
- Open https://console.firebase.google.com/ and create a project.
- Project settings -> add a Web app (</>) and copy its config.
- Open www/app.js and replace firebaseConfig placeholders.
- Build -> Authentication -> Get started -> Sign-in method -> enable Email/Password.
- Build -> Firestore Database -> Create database.
- Paste firestore.rules into Firestore -> Rules and Publish.

2) Run website on a computer
- Install Node.js LTS from https://nodejs.org/
- In the project folder, run: npm install
- Then run: npm run start
- Open the local URL printed in the terminal.
- For public hosting, run npm run build and deploy the dist folder to Firebase Hosting or another HTTPS static host.

3) Android APK (computer required)
- Install Android Studio and Android SDK.
- In project folder run:
  npm install
  npm run build
  npx cap add android
  npx cap sync android
  npx cap open android
- In Android Studio wait for Gradle sync, then Build -> Build Bundle(s) / APK(s) -> Build APK(s).

Important limitations
- This is a starter, not a complete WhatsApp clone. It has no phone OTP, voice/video calls, end-to-end encryption, image uploads, push notifications, password-reset UI, block/report, or groups.
- Firebase free tier has usage limits; not unlimited. Test rules carefully before inviting people.
- Never use open read/write rules or put service-account private keys in frontend code.
- APK building normally requires a computer with Android Studio; this ZIP is not itself an APK.
