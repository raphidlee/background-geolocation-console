# Background Geolocation Console

> A simple Node server & web app with SQLite database for field-testing & analysis of the [Background Geolocation plugin](https://github.com/transistorsoft/cordova-background-geolocation-lt).

![](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/background-geolocation-console-map.png)

![](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/background-geolocation-console-grid.png)

## Running

You must have [npm](https://www.npmjs.org/) installed on your computer.
From the root project directory run these commands from the command line:

```bash
$ npm install
```

## Client & Server

This app hosts two servers:  one for the backend (port 9000) and other to serve the client web app (port 9001).  You need to boot both, in two separate terminal windows:

In one terminal window, boot the backend server:

```bash
$ npm run server
```

And in another terminal window, boot the frontend web app:

```bash
$ npm run client
```

A browser window will automatically launch the front-end web app.

## Configure The Sample App

The Background Geolocation [Sample App](https://github.com/transistorsoft/cordova-background-geolocation-SampleApp) is perfect for use with this web-application.  To configure the app, simply edit `Settings->url` and set it to `http://<your.ip.ad.dress>:9000/locations`.

![](https://dl.dropboxusercontent.com/u/2319755/cordova-background-geolocaiton/settings-url.png)

You should also configure `Settings->autoSync` to `false` while out field-testing as well, so that the app doesn't try syncing each recorded location to the server running on your `localhost`.  Once you return after a test and you're back on your office Wifi, click the **[Sync]** button on the `Settings` screen to upload the cached locations to the **Background Geolocation Console** server.

## Credit

Chris Scott of [Transistor Software](http://transistorsoft.com)

## License

BSD-licensed.
