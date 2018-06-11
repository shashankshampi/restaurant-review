### Installation

`npm i` or `yarn install` in the root of the project.

### How to run the app

In the dist folder, start up an HTTP server of your preference. For example:
`python -m http.server`, if python 3 is installed on your machine. 

### Where is the app running

The local server pipes the site to http://localhost:8000. 

### Backend server

The backend server needs to be run in a separate app. Git-clone the app from:
https://github.com/akolybelnikov/mws-restaurant-stage-3 

Next, follow the steps described in the readme.md of the app.

Alternatively, you can consume the API from the deployed backend at heroku like so:

For restaurants: https://reviews-staging.herokuapp.com/restaurants

For reviews: https://reviews-staging.herokuapp.com/reviews

In this case you don't have to clone and install the sails app, just uncomment lines 65 and 74 and comment out lines 64 and 73 in the DBHelper.js.

The backend at Heroku follows the same API conventions as the sails app, so have a look at the readme.md anyways.

### How to compile static assets

After you have installed the node_modules, in the root of the application run `gulp critical`. Note: should your terminal not recognize the `gulp` command, you would need to install Gulp globally as well: `npm install -g gulp`.

After the assets have been compiled in the /dist folder, the following modifications to the static assets have to be done:

- in the dist forlder, rename `index-critical.html` to `index.html` and `restaurant-critical.html` to `restaurant.html`; original html files in the dist folder need to be removed.

- in `index.html` and `restaurant.html` the link to the script `idb.js` has to be adjusted to point to the minified file in the /lib:     `"lib/idb.js"`;

- finally, the `self.importScripts("node_modules/idb/lib/idb.js")` in the minified sw.js file has to be adjusted to point to the minified idb scribt as well: `self.importScripts("lib/idb.js")`


### Contributions

Are very welcome! For documentation improvements and suggestions, as well as new features:

Fork it!
Create your feature branch: git checkout -b my-new-feature
Commit your changes: git commit -am 'Add some feature'
Push to the branch: git push origin my-new-feature
Submit a pull request :D 


### License

The MIT License (MIT)

Copyright (c) 2018 Andrey Kolybelnikov

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
