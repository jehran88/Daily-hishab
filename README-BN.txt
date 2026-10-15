DAILY HISAB — iPhone setup

1. Firebase Console > Project settings > Your apps থেকে Web App config কপি করুন।
2. firebase-config.js ফাইলে PASTE_... জায়গাগুলো নিজের config দিয়ে বদলান।
3. Firestore Database > Rules-এ firestore.rules-এর নিয়ম বসিয়ে Publish করুন।
4. Authentication > Sign-in method-এ Email/Password enabled রাখুন।
5. GitHub repository-তে ZIP-এর সব ফাইল upload করুন।
6. Repository > Settings > Pages > Deploy from a branch > main > /(root) > Save।
7. Pages-এর URL খুলে পরীক্ষা করুন।

সীমাবদ্ধতা: এই starter-এ লগইন ও প্রতিটি ব্যবহারকারীর আলাদা আয়-খরচ সেভ হয়। পরিবারের একাধিক সদস্যের একই হিসাব শেয়ার করার household/invite সুবিধা এখনো নেই; পরের ধাপে সেটি যোগ করতে হবে। অফলাইনে app shell খোলে, কিন্তু নতুন হিসাব অফলাইনে সেভ হয় না।
নিরাপত্তা: Rules-এ allow read, write: if true দেবেন না। Firebase config browser-এ দেখা যায়, তাই Authentication ও Rules-ই ডেটার নিরাপত্তা নিশ্চিত করবে।
