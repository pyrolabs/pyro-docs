# Interest Page Tutorial

This tutorial will cover setting up a basic app that is a page that allows users to signup for more information for your app. We find that with most projects/startups this is a good place to start your web presence.

## 1. Creating the App

Create a new app by typing the name into the text box. The App in this example will, surprisingly enough, be called ** *exampleApp* **.


## 2. Opening The Code

Now that you have created a new app you can see all of the pages that are described in the [Introduction](). For this example we will start by going into the editor panel.

Once you have the editor tab open click on the folder entitled **Components**. This is where all of the seperate pieces (called compoents) of your app are contained. We will be editing the **Landing** component, so go ahead and open the `landing-index.html` file within the landing component folder.

<!-- Talk about controller being logic and index being main view  -->

## 3. Creating Inputs

Accepting information from a user will require text boxes into which the user will enter the data. We will be adding two text boxes, one for name and another for email. Add these text boxes by copying and pasting this code into `landing-index.html` that you opened in step two:


````html
<div class="list">
<label class="item item-input">
<input type="text" placeholder="Name" ng-model="data.name">
</label>
<label class="item item-input">
<input type="text" placeholder="Email" ng-model="data.email">
</label>
<button class="button button-block button-positive" ng-click="acceptEmail()">
Signup
</button>
</div>
````

Your changes are saved automatically, but we want to see these new changes! You can save the new additions to your live app by clicking the orange cloud button on the right.

<!-- [COMING SOON]  are visible in the Development version of your app which is located in the Tester tab  Development version preview is also available in the Tester tab .-->

Side Note: If you would to learn more about what is going on here checkout the [Intro to Angular]

## 4. Storing Information

The [Pyro Library](https://s3.amazonaws.com/pyro-labs/docs/library/current/Pyro.html) allows you to easily accept information from users and securely store that data. To accomplish this we will be using the `createObject` function from the library by placing the following code into the ** Landing Controller ** (`landing-controller.js`) :

````javascript
// Set empty data
$scope.data = {};

  // Accept email function
  $scope.acceptEmail = function(){
    pyroService.createObject('landing', $scope.data);  
  }
  ````
  Your changes are saved automatically, but we want to see these new changes! You can save the new additions to your live app by clicking the orange cloud button on the right.

  ## 5. Testing It Out

  We are now ready to test out our new page! There are multiple ways to view your live app:
  * Open the Tester panel to view your live app in Pyro
  * Click on the link at the top of the Insights page to view separately in your browser

  Now when you, or anyone else, enters a name and an email in your landing page, that information is stored in your app's own personal database (which only you have access to).

  ### Congratulations on building your first hybrid web application!

  
