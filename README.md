RFduino Scavenger Hunt
=====================

This project is a cordova mobile app built with ionic and angular. The mobile application is a scavenger hunt game. The mobile app works in conjunction with 3 or more RFduinos. Information on RFduino can be found [here](http://www.rfduino.com/). Communication between the mobile app and the RFduinos is done via BLE ([Bluetooth Low Energy](http://en.wikipedia.org/wiki/Bluetooth_low_energy)). Players start the scavenger hunt by checking in with one of the RFduinos as an entry point. The items to be collected (resources) are transferred to the mobile app at the entry point. The mobile app uses the signal strength (RSSI) of the resource (RFduino) to give the player a general idea of the resource's proximity. Once the player gets close to the resource (around 2 feet) the player can 'collect' the resource by connecting directly to the RFduino. At any time the player can proceed to the checkout point (checkout RFduino). Based on the time spent and the number of resources collected the RFduino can be used to actuate some physical feedback. 

## Using this project

It is recommended that you have the following utilities installed: `cordova`, `ionic`, `sass`, and `gulp`. If you are on OS X the Ruby gem installer should already be installed. If you are on Windows go [here](http://www.rubyinstaller.org/) to install. This will allow you to install Sass ([more info on installing Sass](http://sass-lang.com/install)). Use the following commands to install the recommended utilities:
```bash
$ sudo gem install sass
$ sudo npm install -g cordova ionic gulp
```

For more info on Cordova: [Apache Cordova Documentation](http://cordova.apache.org/docs/en/3.5.0/index.html).
For more info on Ionic: [Ionic Getting Started](http://ionicframework.com/getting-started) page.
For more info on Sass: [Sass Guide](http://sass-lang.com/).
For more info on Gulp: [gulp.js](http://gulpjs.com/).

## Installation

While we recommend using the `ionic` utility to create new Ionic projects, you can use this repo as a barebones starting point to your next Ionic app.

To use this project as is, first clone the repo from GitHub, then run:

```bash
$ cd ionic-app-base
$ sudo npm install -g cordova ionic gulp
$ npm install
$ gulp install
```

## Using Sass (optional)

This project makes it easy to use Sass (the SCSS syntax) in your projects. This enables you to override styles from Ionic, and benefit from
Sass's great features.

Just update the `./scss/ionic.app.scss` file, and run `gulp` or `gulp watch` to rebuild the CSS files for Ionic.

Note: if you choose to use the Sass method, make sure to remove the included `ionic.css` file in `index.html`, and then uncomment
the include to your `ionic.app.css` file which now contains all your Sass code and Ionic itself:

```html
<!-- IF using Sass (run gulp sass first), then remove the CSS include above
<link href="css/ionic.app.css" rel="stylesheet">
-->
```

## Updating Ionic

To update to a new version of Ionic, open bower.json and change the version listed there.

For example, to update from version `1.0.0-beta.4` to `1.0.0-beta.5`, open bower.json and change this:

```
"ionic": "driftyco/ionic-bower#1.0.0-beta.4"
```

To this:

```
"ionic": "driftyco/ionic-bower#1.0.0-beta.5"
```

After saving the update to bower.json file, run `gulp install`.

Alternatively, install bower globally with `npm install -g bower` and run `bower install`.

#### Using the Nightly Builds of Ionic

If you feel daring and want use the bleeding edge 'Nightly' version of Ionic, change the version of Ionic in your bower.json to this:

```
"ionic": "driftyco/ionic-bower#master"
```

Warning: the nightly version is not stable.


## Issues
Issues have been disabled on this repo, if you do find an issue or have a question consider posting it on the [Ionic Forum](http://forum.ionicframework.com/).  Or else if there is truly an error, follow our guidelines for [submitting an issue](http://ionicframework.com/contribute/#issues) to the main Ionic repository. On the other hand, pull requests are welcome here!

