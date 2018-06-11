# Restaurant Review App

This app  is created as part of the Udacity Nanodegree "Mobile Web Specialist". The project is divided into three stages.

![Screenshot](Screenshot.png)

#### Stage 1 focuses on 

- accessibility
- responsiveness
- offline first

#### Stage 2 focuses on

- performance
- accessibility
- offline first with IDB


#### Stage 3 focuses on 

- POST requests with offline-first approach
- a form to submit data
- performance ([Lighthouse](https://developers.google.com/web/tools/lighthouse/) performance >90)

## Features

- View all restaurants
- View restaurants for a specific district or cuisine
- View details to a restaurant like opening hours and reviews
- Write reviews for a restaurant
- Mark a restaurant as favorite
- View already loaded pages also in offline mode
- Accessibility: Use the app with screen reader or keyboard-only

## Installation and run locally

1. First this repository.
2. Clone this repository to your desktop.
3. Open the root folder of the repository in a terminal
4. Run `npm i`
5. Check your python version by `python -V`
6. Start local server:
	- For Python 2.x: `python -m SimpleHTTPServer 8000`
	- For Python 3.x: `python3 -m http.server 8000`
7. Provide data from node server (see below)
8. Visit [http://localhost:8000](http://localhost:8000)

## Data from node server

```
$ git clone https://github.com/udacity/mws-restaurant-stage-3.git
$ cd mws-restaurant-stage-3
$ npm i
$ npm i sails -g
$ node server
```

**This server must be up and running parallel to the Python server.**

## Licence

The contents of this repository are covered under the [MIT License](https://github.com/udacity/ud777-writing-readmes/blob/master/LICENSE).
