# Firebase Cloud Messaging (FCM) - Web Push Notifications in Next.js

Implementing desktop notifications using service workers with Firebase Cloud Messaging (FCM) in a Next.js application.

![image](https://github.com/user-attachments/assets/1aae43a0-cffc-4e4f-9777-1b124072b5c2)

> **Note**: Even if the code is correct, ensure that your browser's notification permissions are enabled. If desktop/background notifications are not working, check the notification permissions in your browser settings.

## Steps to Integrate Firebase Cloud Messaging

### 1. Get the Firebase Configuration

Retrieve the Firebase configuration from your Firebase project settings:
- Go to your Firebase project settings.
- Navigate to **SDK setup and configuration**.
- Copy the Firebase config snippet from there.

### 2. Add Firebase Configuration to `firebase-messaging-sw.js`

Place the Firebase configuration in the `firebase-messaging-sw.js` file located in the `public` folder of your Next.js project. Note that service workers cannot access environment variables from `.env` files, so you need to include the configuration directly.

```javascript
// public/firebase-messaging-sw.js

const firebaseConfig = {
  apiKey: "AIzaSyDwdTWcNktQmMrBQmwl7mSMO10",
  authDomain: "habbit-bb11baseapp.com",
  projectId: "habbder-b11e6",
  storageBucket: "habbit-buile6.appspot.com",
  messagingSenderId: "940229275",
  appId: "1:940221075:web:fde088d062f59fe",
  measurementId: "G-SGRX2V9",
};

 3) get "vapid key" from project settings>service accounts>generate key

4. get "service_key.json" from project settings>service accounts>generate key
