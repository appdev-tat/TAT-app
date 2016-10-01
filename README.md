# Truckers Against Trafficking mobile app

An app for Truckers Against Trafficking, built with [PhoneGap](http://phonegap.com/) and [Ionic](http://ionicframework.com/).

## Developing instructions

### Setting up a dev environment

Use git to clone the repo to a directory of your choice:
```sh
$ git clone https://github.com/ransoing/TAT-app.git
```

Install [Node.js](https://nodejs.org/en/).

In a terminal or command console, navigate to the repo directory and run:
```sh
$ npm install -g phonegap
$ npm install -g ionic
$ npm install
```

PhoneGap apps are essentially just websites that run as a native app, so you can develop like you would for a regular website. Ionic has a nifty tool to let you see what the app looks like on both iOS and Android simultaneously. In a console, in the project directory, run:
```sh
$ ionic serve --lab
```

To easily test the app on a real device, download the PhoneGap desktop app and the PhoneGap developer app for mobile devices. See the [PhoneGap](http://phonegap.com/) website for details on how to make this magic work.

### Building the app

When you're happy with the changes you've made to the app, use git to commit and push your changes to github. Then log into [PhoneGap Build](https://build.phonegap.com/), and tell it to update from github and rebuild the app.

## Other things to note

I think Ionic has a built-in way to generate all the necessary icon sizes automatically, but I used [http://pgicons.abiro.com/](http://pgicons.abiro.com/). If you need to make changes to the app icon, use this tool to generate files that match the filenames of the current icons.
