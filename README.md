## Firebase
https://console.firebase.google.com/
```bash
# tutorial:https://www.youtube.com/watch?v=esIbvCxJsag&list=PL7I8MmpG2FCCU60S6nkZUqJqet68VaMdi&index=1
# https://www.youtube.com/watch?v=eM71Ez6xG-I&list=PL7I8MmpG2FCCU60S6nkZUqJqet68VaMdi&index=2&t=206s
```
```javascript
// web client
// javascript version 8: source demo: https://drive.google.com/drive/folders/19_uCGlrjapL6Wc52g0k3xngBBCn6Eg58
// javascript version 9: https://firebase.google.com/docs/database/web/read-and-write?authuser=0#web-version-9_1
// console: https://console.firebase.google.com/u/0/project/peaceful-web-290106/database/peaceful-web-290106-default-rtdb/data
<script type="module">
  // Import the functions you need from the SDKs you need
  import { initializeApp } from "https://www.gstatic.com/firebasejs/9.6.1/firebase-app.js";
  import { getAnalytics } from "https://www.gstatic.com/firebasejs/9.6.1/firebase-analytics.js";
  // TODO: Add SDKs for Firebase products that you want to use
  // https://firebase.google.com/docs/web/setup#available-libraries

  // Your web app's Firebase configuration
  // For Firebase JS SDK v7.20.0 and later, measurementId is optional
  const firebaseConfig = {
    apiKey: "AIzaSyCrCnYxXL46MLRpai4ODDBB8IMRqKWjsCs",
    authDomain: "peaceful-web-290106.firebaseapp.com",
    databaseURL: "https://peaceful-web-290106-default-rtdb.firebaseio.com",
    projectId: "peaceful-web-290106",
    storageBucket: "peaceful-web-290106.appspot.com",
    messagingSenderId: "99608514754",
    appId: "1:99608514754:web:a6f62a56289e09488d6b5b",
    measurementId: "G-6H1LZ344HY"
  };

  // Initialize Firebase
  const app = initializeApp(firebaseConfig);
  const analytics = getAnalytics(app);
</script>
```
```javascript
// nodejs: https://console.firebase.google.com/u/0/project/peaceful-web-290106/settings/serviceaccounts/adminsdk

var admin = require("firebase-admin");

var serviceAccount = require("/Users/datdao/Downloads/peaceful-web-290106-firebase-adminsdk-l7jul-17a4ef3c96.json");

admin.initializeApp({
  credential: admin.credential.cert(serviceAccount),
  databaseURL: "https://peaceful-web-290106-default-rtdb.firebaseio.com"
});

```

```bash
# ssh/.config
Host github.com
  User datagit
  Hostname github.com
  PreferredAuthentications publickey
  IdentityFile /home/user/.ssh/id_rsa_for_github.com
```