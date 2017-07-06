Waundr
=====================

A real time social walking experience. A deployed version of the demo can be accessed at: www.waundr.com

### How it works

Users can log in using either Facebook or Google.

!["Screenshot of the landing page"](https://github.com/ffiargus/Waundr/blob/master/gif/login.png)

After logging in, users can create markers and they will broadcast to others users in real time using websockets.

!["Gif for creating marker"](https://github.com/ffiargus/Waundr/blob/master/gif/Createmarkers.gif)

The app fetches data from the Meetups api so it is already populated with some markers on initial use.
In addition the users can also confirm the event by clicking on the number or reject the event by clicking on the 'X', events are time limited to 2 hours, however confirms will refresh the timer, and rejects will remove the marker prematurely.

!["Gif for meetup"](https://github.com/ffiargus/Waundr/blob/master/gif/meetup.gif)

The app also allows users to filter events near you. You can do this by the filter button at the bottom right hand corner.

!["Gif for filter"](https://github.com/ffiargus/Waundr/blob/master/gif/filter.gif)

Mobile Versions

!["Example of iOS and Android devices"](https://github.com/ffiargus/Waundr/blob/master/gif/MobileExample.png)

### Loading Waundr

In order to run the app, you must first create a .env file.
The .env file is for authentication for google and facebook and linking it with the postgres server.

```
DB_HOST=
DB_USER=
DB_PASS=
DB_NAME=
DB_SSL=
DB_PORT=5432

CLIENTID="Google ID"
CLIENTSECRET="Google Client secret"

APPID="Facebook ID"
APPSECRET="Facebook Secret"

```

Open a terminal and enter the following commands

```
npm install, // to install the dependencies
npm start
open http://localhost:3000

```

In order to get the server working. Open another terminal and enter the following commands.

```
cd production
npm install
npm start
```

In order to get the mobile version working.

```
cd veronica
npm install
react-native run-ios; // react-native run-andriod
```

### Dependencies

* React
* Webpack
* [babel-loader](https://github.com/babel/babel-loader)
* [webpack-dev-server](https://github.com/webpack/webpack-dev-server)
* express": "^4.15.3",
* hover.css": "^2.2.0",
* jquery": "^3.2.1",
* material-ui": "^0.18.3",
* materialize-css": "^0.98.2",
* passport-facebook": "^2.1.1",
* passport-twitter": "^1.0.4",
* prop-types": "^15.5.10",
* react": "15.4.2",
* react-dom": "15.4.2",
* react-materialize": "^1.0.1",
* react-router": "^4.1.1",
* react-router-dom": "^4.1.1",
* redis": "^2.7.1",
* ws": "3.0.0"
* "body-parser": "^1.17.2",
* "connect-flash": "^0.1.1",
* "cookie-parser": "^1.4.3",
* "cors": "^2.8.3",
* "dotenv": "^4.0.0",
* "express-session": "^1.15.3",
* "node-craigslist": "^1.1.2",
* "passport": "^0.3.2",
* "passport-facebook": "^2.1.1",
* "passport-google-oauth": "^1.0.0",
* "pg": "^6.3.1",
* "pg-hstore": "^2.3.2",
* "redis": "^2.7.1",
* "request-promise": "^4.2.1",
* "sequelize": "^4.1.0",
* "google-map-react": "^0.24.0",
* "react": "^15.6.1",
* "react-native": "0.45.1",
* "react-native-deprecated-custom-components": "^0.1.0",
* "react-native-maps": "^0.15.2",
* "react-native-material-kit": "^0.4.1",
* "react-native-pulse": "^1.0.4",
* "react-redux": "^5.0.5",
* "redux": "^3.7.1"
