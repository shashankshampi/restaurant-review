
-# Restaurant Review App
+# Mobile Web Specialist Certification Course
+---
+#### _Three Stage Course Material Project - Restaurant Reviews_
 
-This app  is created as part of the Udacity Nanodegree "Mobile Web Specialist". The project is divided into three stages.
+## Project Overview: Stage 1
 
-![Screenshot](Screenshot.png)
+For the **Restaurant Reviews** projects, you will incrementally convert a static webpage to a mobile-ready web application. In **Stage One**, you will take a static design that lacks accessibility and convert the design to be responsive on different sized displays and accessible for screen reader use. You will also add a service worker to begin the process of creating a seamless offline experience for your users.
 
-#### Stage 1 focuses on 
+### Specification
 
-- accessibility
-- responsiveness
-- offline first
+You have been provided the code for a restaurant reviews website. The code has a lot of issues. It’s barely usable on a desktop browser, much less a mobile device. It also doesn’t include any standard accessibility features, and it doesn’t work offline at all. Your job is to update the code to resolve these issues while still maintaining the included functionality. 
 
-#### Stage 2 focuses on
+### What do I do from here?
 
-- performance
-- accessibility
-- offline first with IDB
+1. In this folder, start up a simple HTTP server to serve up the site files on your local computer. Python has some simple tools to do this, and you don't even need to know Python. For most people, it's already installed on your computer. 
 
+In a terminal, check the version of Python you have: `python -V`. If you have Python 2.x, spin up the server with `python -m SimpleHTTPServer 8000` (or some other port, if port 8000 is already in use.) For Python 3.x, you can use `python3 -m http.server 8000`. If you don't have Python installed, navigate to Python's [website](https://www.python.org/) to download and install the software.
 
-#### Stage 3 focuses on 
+2. With your server running, visit the site: `http://localhost:8000`, and look around for a bit to see what the current experience looks like.
+3. Explore the provided code, and make start making a plan to implement the required features in three areas: responsive design, accessibility and offline use.
+4. Write code to implement the updates to get this site on its way to being a mobile-ready website.
 
-- POST requests with offline-first approach
-- a form to submit data
-- performance ([Lighthouse](https://developers.google.com/web/tools/lighthouse/) performance >90)
+### Note about ES6
 
-## Features
+Most of the code in this project has been written to the ES6 JavaScript specification for compatibility with modern web browsers and future proofing JavaScript code. As much as possible, try to maintain use of ES6 in any additional JavaScript you write. 
 
-- View all restaurants
-- View restaurants for a specific district or cuisine
-- View details to a restaurant like opening hours and reviews
-- Write reviews for a restaurant
-- Mark a restaurant as favorite
-- View already loaded pages also in offline mode
-- Accessibility: Use the app with screen reader or keyboard-only
 
-## Installation and run locally
 
-1. First this repository.
-2. Clone this repository to your desktop.
-3. Open the root folder of the repository in a terminal
-4. Run `npm i`
-5. Check your python version by `python -V`
-6. Start local server:
-	- For Python 2.x: `python -m SimpleHTTPServer 8000`
-	- For Python 3.x: `python3 -m http.server 8000`
-7. Provide data from node server (see below)
-8. Visit [http://localhost:8000](http://localhost:8000)
-
-## Data from node server
-
-```
-$ git clone https://github.com/udacity/mws-restaurant-stage-3.git
-$ cd mws-restaurant-stage-3
-$ npm i
-$ npm i sails -g
-$ node server
-```
-
-**This server must be up and running parallel to the Python server.**
-
-## Licence
-
-The contents of this repository are covered under the [MIT License](https://github.com/udacity/ud777-writing-readmes/blob/master/LICENSE).
