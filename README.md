# Geoguess Master

![logo](../master/public/img/icons/android-icon-192x192.png)

https://geoguessmaster.com/

### About
Free and lazy geoguess game with no ads. 
Players compete how close the player can guess random locations in five rounds. 
You can share the score with other people via social media like Facebook or Twitter. 
You can play multiplayer game with your friends up to five friends. 
The first player creates a room and decide the room size. 
Other players type the same room name as the first player created and the game will start. 

### Build Setup
You need to configure Google Maps Platform and Firebase to make game work. 
See the instructions below. 

- [Google Maps API](https://developers.google.com/maps/documentation/javascript/get-api-key#get-the-api-key)  
- [Firebase](https://firebase.google.com/docs/database/web/start)  
- [Firebase Realtime Database](https://firebase.google.com/docs/database/web/start)
 
Once you get an API key and register the project with Firebase, create files named `.env.development.local` and `.env.production.local` inside this project to put environment variables. 
The files should be like this. 

`.env.production.local`
```
NODE_ENV=production
VUE_APP_API_KEY=YOUR_GOOGLE_MAPS_API_KEY
VUE_APP_FIREBASE_API_KEY=YOUR_FIREBASE_API_KEY
VUE_APP_FIREBASE_PROJECT_ID=YOUR_FIREBASE_PROJECT_ID
VUE_APP_FIREBASE_MESSAGING_SENDER_ID=YOUR_FIREBASE_MESSAGING_SENDER_ID
VUE_APP_FIREBASE_APP_ID=YOUR_FIREBASE_APP_ID
VUE_APP_FIREBASE_MEASUREMENT_ID=YOUR_FIREBASE_MEASUREMENT_ID
```

`.env.development.local`
```
NODE_ENV=development
...
```

Now you can run this game.  
Download Node.js [here](https://nodejs.org/en/download/) if you don't have and make sure you can run `npm` from the terminal.

```
# install dependencies
npm install

# run locally
npm run serve

# build for production
npm run build
```

You need to host this project as a static website to play multiplayer game with your friends. I recommend using [Netlify](https://www.netlify.com/). You can just fork this project and deploy it from Netlify. Also you can manage environment variables on the Netlify console.

### Features
- Free game with no ads
- Multiplayer game
- PWA and responsive design

### Contributors
[Paulo Gomes](http://www.pauloxgomes.com/), UI design  

### License
Licensed under [MIT License](https://github.com/spider-hand/Geoguess-Master-Web/blob/master/LICENSE)

### Contact
Feel free to give me feedback.  

creative.spider.hand@gmail.com  
or  
[Discord](https://discord.gg/fPpUzgJ)
