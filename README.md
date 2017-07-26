# AngularJS


![toomanyframeworks](https://cdn.meme.am/instances/61726473.jpg)

## What is Angular?
* JavaScript framework for building dynamic web applications
* Built with CRUD applications in mind (i.e. not for applications with lots of big DOM changes --> games)
* Intended to 'close the gap' between HTML and JS
* Isolates an application's responsibilities from each other
  * *Decouples DOM manipulation from app logic*
  * Examples: receiving data, manipulating DOM, etc.
* Utilizes declarative programming
* Reduces need for jQuery (esp. with form data)

## Angular's Structure
* MVC (but not strict MVC)
  * View: HTML page
  * View/Model (Controller): Updates the view if there are changes to the model, and updates the model if there are changes made to the view <-- *data binding* (keeps data synchronized between the two)
  * Model 
* **Directives** (super important!!)
  * Custom HTML that can be used to manipulate the DOM
  * Makes it easier to develop interactive elements on the page
  * Start with `ng-`
  * Examples: attaching a click handler, appending items to a list
* Everything in Angular is inside a **module**
  * Similar to modules in Ruby
  * Containers for different parts of an app (e.g. controllers, filters, directives)
  * Each module contains a set of related functions
  * Modules should be made for each feature and each reusable component

## High Level View
1. Declare a click event on an element
2. Write logic for the click event in the controller
3. Pass data from controller to view
4. View uses directives to manipulate DOM (i.e. Angular manipulates the DOM instead of you doing it directly)
  
## When to Use Angular
* Building client-side single-page applications
  * Gmail, Facebook, Twitter
* Basically any CRUD app
  * Helps reduce the amount of code you have to write by eliminating most boilerplate and AJAX calls
  
## Example
```
<!DOCTYPE html>
<html ng-app>
  <head>
    <title>My AngularJS Blog</title>
    <script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.5.6/angular.min.js"></script>
  </head>
  <body>
   <form>
    <input ng-model="title" type="text"/>
    <textarea ng-model="body"></textarea>
    <input type="submit" value="Post article" />
   </form>
   <div class="article">
    <div>{{ title }}</div>
    <p>{{ body }}</p>
   </div>
  </body>
</html>
```
* The value of the ng-model attribute on the text inputs matches the values inside the curly braces
  * The content of the form elements is automatically written to the page where the corresponding curly braces are
  
## Angular vs. React
* Angular puts JS into HTML; React puts HTML into JS
* Angular is more robust than React (but React isn't exactly a framework, so this comparison is a bit subjective)
* React requires less code and has better performance

![toomanyframeworks2](https://cdn-images-1.medium.com/max/1600/1*k67k1BGo3vIPLInrldsJAw.jpeg)
