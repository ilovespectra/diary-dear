# dear diary

the journal you won't lose next time you move.

[demo here](https://journal-app-ea7ec.web.app/index.html)<br>
*the password for view entries is* 
```
YOUR_PASSWORD
```

## Prerequisites

Before you begin, ensure you have the following prerequisites installed on your machine:

0. **Firebase Account**: Create a free Firebase account at [Firebase](https://firebase.google.com/) if you don't already have one.

1. **Node.js and npm**: Download and install Node.js and npm from [Node.js](https://nodejs.org/). This will also install the Node Package Manager (npm).

2. **npm install**

```
npm install 
```

3. **Firebase CLI**: Open your terminal or command prompt and run the following command to install the Firebase Command Line Interface:

   ```
    npm install -g firebase-tools
   ```

4. **create a new project on firebase**

![add project](https://cdn.discordapp.com/attachments/1051281685234327613/1153856428935761920/Screenshot_2023-09-19_at_6.47.09_PM.png)<br>
enable analytics, use default account

![add firebase to webpage](https://cdn.discordapp.com/attachments/1051281685234327613/1153856428633763861/Screenshot_2023-09-19_at_6.49.39_PM.png)<br>
add firebase to your webpage, setup hosting

![add firebase to your webapp](https://cdn.discordapp.com/attachments/1051281685234327613/1153856428264656956/Screenshot_2023-09-19_at_6.49.48_PM.png)

5. **setup your project**

run 
```
npm install firebase
```

![config](https://cdn.discordapp.com/attachments/1051281685234327613/1153856428013015081/Screenshot_2023-09-19_at_6.50.06_PM.png)

6. **deploy to firebase hosting**

![deploy to firebase hosting](https://cdn.discordapp.com/attachments/1051281685234327613/1153857967591002162/image.png)

7. **add firestore storage**

   select `Build`, and select `Firestore Database`

![add firestore](https://cdn.discordapp.com/attachments/1051281685234327613/1153858693675352064/image.png)

8. **enable read/write permissions**

change to true and hit publish

![true](https://cdn.discordapp.com/attachments/1051281685234327613/1153858763049152665/image.png)

9. **init firebase**

```
firebase init
```

10. **configure as follows**

Here is what your firebase config will look like:

![add firebase to web app](https://cdn.discordapp.com/attachments/1051281685234327613/1154039834248216637/image.png)

replace the following `const` with your config:
```
// This is the configuration provided by Firebase
        const firebaseConfig = {
            apiKey: "YOUR_API_KEY",
            authDomain: "YOUR_AUTH_DOMAIN",
            projectId: "YOUR_PROJECT_ID",
            storageBucket: "YOUR_STORAGE_BUCKET",
            messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
            appId: "YOUR_APP_ID",
            measurementId: "YOUR_MEASUREMENT_ID"
        };
```

modify your firebase configuration in the `am.html`, `pm.html`, `freewrite.html`, and `view_entries.html` pages. find this in your script and replace it with your firebase configuration provided when you selected 'Add Firebase to Web App'.

![configure as follows](https://cdn.discordapp.com/attachments/1051281685234327613/1153863272295047168/image.png)

select `add to existing project` and select the project you just setup in firebase. 

setup firesore, follow these responses carefully:

![firestore](https://cdn.discordapp.com/attachments/1051281685234327613/1153863374136950845/image.png)

11. **deploy**

```
firebase deploy --only hosting   
```
