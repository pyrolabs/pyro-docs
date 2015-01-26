# How Pyro Works

## Built With

We use the power of some of the best Frameworks/Libraries/Projects available to power **Pyro**:

* [Firebase](http://firebase.com)
* [Ionic](http://ionicframework.com)
* [Nodejs](http://nodejs.org/) by Joyent
* [AngularJS](http://angularjs.org) by Google
* [AngularFire](https://www.firebase.com/docs/web/libraries/angular/api.html) by Firebase

The power of Firebase's realtime and security features allows us to offload almost all of the logical functionality of Pyro to the client side. For us this means limited server costs, and for the user it means faster load times and more actions available offline.

Ionic Framework's native looking CSS/Javascript gives apps the smooth native feel from the start.

## System Architecture

### Platform

* Client communicating with Firebase and Server
* Functionality from library
* Service for Angular

*More Coming Soon*

<!-- Diagram showing Client/Firebase/Server Layout -->

### Server

* Request/Worker layout with focus on modularity
* Standardized addition of new features (open source modules)
* Task automation (versioning/deploying)

*More Coming Soon*

### Library

Much like the javascript library that Firebase has built, the Pyro Library allows for easy storage of app data.

Draw initial parallel to Firebase library then describe how this is higher level

* Session/Presense Management
* Time stamping objects
* Roll Management
* Angular Service

<!-- Diagram showing Server/Worker layout -->

## Structure

* Fractal/Component Pattern
* Angular Modules (Factory/Service)


### Future plans
* Push notification
* Saving bound objects (FAT Binding)
* multiple account types

## Functional Landscape

### Signup

When you signup with Pyro you also create a new account with Firebase. This is done so that you can manage your application's databases separately if you would like.

If you already have a Firebase account associated with your Signup email then you will be directed to log in to that account through our site. We are hoping to change this account login method after getting the chance to work directly with Firebase.

### App Generation

* Template app copied
* Automatic hosting/configuration

### Editor Panel

* Firepad
* Upload button
* Folder/File Structure

### Tester Panel

* Different device types/sizes
* Development/Production Environments
* Pyroception

#### Future Plans:

* ng-app in ng-app
* Offsite builds (cordova running compiling on server)
* Automatic Documentation
* Handle Different Environments
