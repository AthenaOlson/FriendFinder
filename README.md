# FriendFinder

Find your best friend match from the cast of characters of The Gilmore Girls in Stars Hollow, CT.

### Heroku live link

https://glacial-depths-97072.herokuapp.com/

### npm packages installed

    * npm install --save express

    * npm install --save body-parser

    * npm install --save path

### About the app

Simply navigate to the home page, and select the 'Survey' button to start the survey that will match you to your best friend match from Stars Hollow. Fill out the form, submit, and the app will return your best match based on your survey answers.

### Requirements

    * Separate files for server logic, storing of friends, views, and routing

    * 10-question survey to assess uniqueness of users

    * Use express, body-parser, and path npm packages in the server.js file

    * Separate JavaScript files for routing (htmlRoutes.js and apiRoutes.js)

    * Appropriate GET and POST routes for serving HTML pages and API calls

    * Separate file for storing friends (friends.js)

    * Calculate best match for user once survey is completed and return that match to the user

### Leveraged Technologies

    * JavaScript

    * jQuery Libray

    * node.js

    * Express.js

    * html

    * bootstrap

    * css

### Code described

    * server.js sets the express server, specifies port #3000, the npm packages to load, routes, which are externalized in apiRoutes.js & htmlRoutes.js

    * 2 separate html files, home.html & survey.html that serve as the front-end portion of the code

    * The best friend match is calculated by the user's survey results vs. the minimal difference in scores of the Stars Hollows friends listed in friends.js, return to a JSON object (viewable click at bottom of home.html & survey.html)

    * A modal displays the best friend match with a picture of the user's best match

    * User's data is printed to the JSON

    * Friend data is stored on friends.js as such:

    {
		name: "Rory Gilmore",
		photo: "http://1l75682k88ng461uk325y9ns.wpengine.netdna-cdn.com/wp-content/uploads/2017/01/Screen-Shot-2017-01-24-at-7.10.12-PM-217x300.png",
		scores: [5, 4, 5, 3, 1, 1, 1, 5, 1, 5]
	},