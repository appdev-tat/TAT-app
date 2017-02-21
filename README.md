# Truckers Against Trafficking mobile app

An app for Truckers Against Trafficking, built with [PhoneGap](http://phonegap.com/) and [Ionic](http://ionicframework.com/).

PhoneGap apps are essentially just websites that run as a native app, so all you need is a little web design knowhow.

## Developing instructions

### Setting up a dev environment

##### Step 1

Use git (either the [command line utility](https://git-scm.com/) or the [github desktop app](https://desktop.github.com/)) to clone the repo to a directory of your choice.

If you use the command line utility:

```sh
$ cd some/directory/
$ git clone https://github.com/appdev-tat/TAT-app.git
```

##### Step 2

Download the PhoneGap desktop app and the PhoneGap developer app for mobile devices. See the [PhoneGap](http://phonegap.com/) website for details.

##### Step 3

Run the PhoneGap desktop app and open the TAT-app project folder. Click the `>` button to start the server.

##### Step 4

Click the IP address at the bottom of the PhoneGap desktop app. This opens up a browser window to display the app. When you make changes to the project files, the browser should automatically refresh to show the changes.

You can also preview the app on a mobile device by running the PhoneGap mobile app. Enter the IP address shown on the desktop app when prompted. Just like the browser on your computer, your mobile device should automatically refresh in response to changes in the project files.

##### Step 5, optional advanced dev environment

Install [Node.js](https://nodejs.org/en/).

In a terminal or command console, navigate to the repo directory and run:

```sh
$ npm install -g phonegap
$ npm install -g ionic
$ npm install
```

Both the phonegap and ionic command line tools have rather nifty features. Ionic has a tool to let you see what the app looks like on both iOS and Android simultaneously. In a console, in the project directory, run:

```sh
$ ionic serve --lab
```

### Project layout

For simple edits, you only need to worry about the files here:

```sh
[project-dir]/www/templates/
```

Each file in that directory represents a different "page" in the app, with the exception of `tabs.html`.

Be aware that apps made with Ionic also use the [Angular framework](https://angularjs.org/).

##### Notes for beginners

Edit the files using any text editor, for example, Notepad. If you want to use something much better, install [Visual Studio Code](https://code.visualstudio.com).

Here's a basic [HTML tutorial](http://www.w3schools.com/html/). Some of it does not apply to this app. For anything beyond what the tutorial covers, get assistance from a web developer.

### Building the app

When you're happy with the changes you've made to the app, use git to commit and push your changes to github. Then log into [PhoneGap Build](https://build.phonegap.com/), and tell it to update from github and rebuild the app.

The `master` branch assumes that Android is the target platform. The `master-ios` branch has an altered `config.xml` file and is suitable for deployment to iOS devices.

## Other things to note

I think Ionic has a built-in way to generate all the necessary icon sizes automatically, but I used [http://pgicons.abiro.com/](http://pgicons.abiro.com/). If you need to make changes to the app icon, use this tool to generate files that match the filenames of the current icons.

When you deploy changes, you should merge those changes into the `master-ios` branch as well. The only difference between `master` and `master-ios` should be the `config.xml` file.