# How Pyro Works


## Built With

We use the power of some of the best Frameworks/Libraries/Projects available to power Pyro:

* [Firebase](http://firebase.com)
* [Ionic](http://ionicframework.com)
* [nodejs]()
* [AngularJS](http://angularjs.org) by Google
* [AngularFire]() by Firebase

and many more.

The power of Firebase's realtime and security features allows us to offload almost all of the logical functionality to the client side of the App.

## Structure

* Fractal/Component Pattern
* Angular Modules (Factory/Service)

## Library

Draw initial parallel to Firebase library then describe how this is higher level

* Session/Presense Management
* Time stamping objects
* Roll Management
* Angular Service

### Future plans
* Push notification
* Saving bound objects (FAT Binding)
* multiple account types

## Functional Landscape

### Signup

When you signup with Pyro you also create a new account with Firebase. This is done so that you can manage your application's databases separately if you would like.

If you already have a Firebase account associated with your Signup email then you will be directed to log in to that account through our site. We are hoping to change this account login method after getting the chance to work directly with Firebase.

### Generation

* Template app copied
* Automatic hosting/configuration

### Editor

* Firepad
* Upload button
* Folder/File Structure

### Tester

* Different device types/sizes
* Pyroception

#### Future Plans:
* ng-app in ng-app
* Offsite builds (cordova running compiling on server)

## Server Infrastructure

* Request/Worker layout with focus on modularity
* Standardized addition of new features
* Task automation (versioning/deploying)
