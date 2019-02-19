# Turn-Down-For-What (TreeHacks 2019)
- An app that utilizes the phone's accelerometer to determine the optimal time for sleeping and waking up


### Description and Inspiration
People often listen to music or a podcast as they head to bed -- something about the extra noise just helps you nod off. But much too often, just about you're doze off, you have to shake yourself awake, just to fiddle with your phone or rip out your headphones. For the sake of a better night sleep, we decided to make an app to rectify this problem.

Our app allows one to use voice commands to start off the in-app music player and accelerometer. The phone then uses the accelerometer to sense as a person falls asleep, gradually turning down the volume, and stopping the audio entire once we've detected you've entered deep sleep (In deep sleep, the body is paralyzed and have a lot less movement). In addition, you can also set an alarm time, where our app will start to look for signs of movement and wakefulness, and begin quietly playing music to wake you up, gradually increasing the volume as the user awakes.

### Technology 
- We used Node.js for back-end and React Native for front-end, utilizing the SoundHound API and Expo.io. The app was created and shipped using Expo.io. We integrated SoundHound voice commands into our app. Because Expo.io cannot use filestreams and SoundHound only takes streams, we had to write a back-end Node.js server to convert a FORM POST to a stream. Also, the back-end server, converts the input audio to the specific format 

### To use
- run `npm install` in both the **Client-Side** folder and the **Server-Side** folder
- Download the expo app 
- run `expo start` in the **Client-Side** folder
- run `node app.js` in the **Server-Side** folder in another terminal
- Scan the QR code on the Expo page that pops up
- Done !


### Links
##### Devpost
https://devpost.com/software/bettersleep-backend
##### Youtube Demo
https://www.youtube.com/watch?v=sdOLNpMO_n0&feature=youtu.be&fbclid=IwAR0CVdZGO8lnZOfZSi-vU4ESLn0cjsKF7bkfgilV_z1AAQA4dU1JWBuKfUQ


Note: this is a copy of the official project for personal references, the git repos that we used for the hackathon is the following:

##### Client-side (front-end)
https://github.com/DavidWChen/BetterSleep

##### Server-side (back-end)
https://github.com/DavidWChen/BetterSleep-Backend




