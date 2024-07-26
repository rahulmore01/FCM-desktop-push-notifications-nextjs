# firebase-cloud-messaging-FCM--web-push-notifications-nextjs

firebase-cloud-messaging(FCM)-web-push-notifications-nextjs - for desktop notifications using service workers
![image](https://github.com/user-attachments/assets/1aae43a0-cffc-4e4f-9777-1b124072b5c2)


Note- even if code is perfect and still destop/background notifications are not working, check notification permissions of your browser.

1. get the firebaseConfig env files from -

<img width="1440" alt="image" src="https://github.com/user-attachments/assets/ec0c3bad-d256-4f69-9fa1-dc1a0ee3541d">

2)put the same env's into "firebase-messaging-sw.js" file in public folder.

note- these are broken use your and dont use process.env.\* because serviceworkers cant access these from .env file

const firebaseConfig = {
apiKey: "AIzaSyDwdTWcNktQmMrBQmwl7mSMO10",
authDomain: "habbit-bb11baseapp.com",
projectId: "habbder-b11e6",
storageBucket: "habbit-buile6.appspot.com",
messagingSenderId: "940229275",
appId: "1:940221075:web:fde088d062f59fe",
measurementId: "G-SGRX2V9",
}; 3) get "vapid key" from project settings>service accounts>generate key
<img width="1440" alt="image" src="https://github.com/user-attachments/assets/333098f0-952a-46b1-9940-cd7d11dc070d">

4. get "service_key.json" from project settings>service accounts>generate key
   <img width="1432" alt="image" src="https://github.com/user-attachments/assets/49dc3b3c-e054-4636-83ef-e0d90a55e51c">
