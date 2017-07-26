# AngularJS


![toomanyframeworks](https://cdn.meme.am/instances/61726473.jpg)

## What is Angular?
* JavaScript framework for building dynamic web applications
* Intended to 'close the gap' between HTML and JS
* Isolates an application's responsibilities from each other
  * *Decouples DOM manipulation from app logic*
  * Examples: receiving data, manipulating DOM, etc.
* Provides bi-directional **dynamic data binding**
  * If your backend data changes, your changes will appear automatically in your view
  * If the data in your view changes, your model will be automatically updated with the changes
* Utilizes declarative programming
* Built with CRUD applications in mind (i.e. not for applications with lots of big DOM changes --> games)

## Angular's Structure
* Controller: stores data (state, behavior)
* View
* **Directives** (super important!!
  * Custom HTML that can be used to manipulate the DOM
  * Makes it easier to develop interactive elements on the page
  * Examples: attaching a click handler, appending items to a list
* Everything in Angular is inside a **module** (more on this below!)

## High Level View
1. Declare that there's a click event on an element
2. Write logic for the click event in the controller
3. Controller passes data to the view
4. View uses directives to manipulate DOM (i.e. Angular manipulates the DOM instead of you doing it directly)

## Modules 
* Similar to modules in Ruby
* Containers for different parts of an app (e.g. controllers, filters, directives)
* Each module contains a set of related functions
* Modules should be made for each feature and each reusable component
  * Can be reused to DRY up code
  
## When to Use Angular
* Building client-side single-page applications
  * Gmail, Facebook, Twitter
* Basically any CRUD app
  * Helps reduce the amount of code you have to write by eliminating most boilerplate and AJAX calls
  
## Example


## Angular vs. React
* Angular puts JS into HTML; React puts HTML into JS
* Angular is more robust than React
* React requires less code and has better performance
