# Project Overview

This project has a web-based application that reads RSS feeds, which includes [Jasmine]. An application with an complete test suite.

# How to access the project

1. Consider the application's HTML (**./index.html**), CSS (**./css/style.css**) and JavaScript (**./js/app.js**).
2. Code testing was focus on Jasmine spec file in **./jasmine/spec/feedreader.js**. Considering aspect are:
   i. Firstly the `allFeeds` variable in **./js/app.js** was edited to make the provided test fail and see how Jasmine visualizes this failure in the application.
   ii. Then the `allFeeds` variable was returned to a passing state.
3. Written tests:
   i. A test that loops through each feed in the `allFeeds` object and ensures it has a URL defined and that the URL is not empty.
   ii. A test that loops through each feed in the `allFeeds` object and ensures it has a name defined and that the name is not empty.
   iii. A new test suite named `"The menu"`.
   iv. A test that ensures the menu element is hidden by default. Also analyze the HTML and the CSS to determine how we're performing the hiding/showing of the menu element.
   v. A test that ensures the menu changes visibility when the menu icon is clicked. The test has two expectations: the menu display when clicked and it hide when clicked again.
   vi. A test suite named `"Initial Entries"`.
   vii. A test that ensures when the `loadFeed` function is called and completes its work, there is at least a single `.entry` element within the `.feed` container.
   viii. A test suite named `"New Feed Selection"`.
   ix. A test that ensures when a new feed is loaded by the `loadFeed` function that the content actually changes.
4. All tests passed. 

