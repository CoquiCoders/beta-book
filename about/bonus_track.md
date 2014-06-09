# Bonus track


1. [I Love Puerto Rico](http://http://www.ilovepuertorico.org/)

We picked up a project on Github called Hackathon Starter. It's a very well documented boilerplate / starter kit for a quick project just like this. It's using Express for the web framework, MongoDB for the database, and quite a few other various and useful packages.

For the front end, it uses the Jade templating language. In addition, we used JQuery Isotope to create all those sleek responsive animations you see when blocks are moving around.
The project has been deployed on Heroku. The only thing we had to install that was not already included in the hackathon starter was a node package called dotenv. It let us maintain a local file with some of the configuration settiongs that I would be setting up in Heroku config variables.

We set up 3 paths in express:

[GET] / -- the main path that renders the barebones pages for all the notes. The view that this calls does not contain any notes yet since they are loaded in via ajax.
[POST] /note/new -- This is the path that the form data from the note creation form gets posted to.
[GET]  /notes/:skip/:limit -- A path that returns notes stored in the database based on a skip and limit parameter. This is what's used to load notes into the page, and also used to load additional notes when the user scrolls to the bottom of the page.

The app has gotten forked by several of the other fellowship teams. It currently lives online at I Love Puerto Rico, and the codebase can be found on GitHub.


2. Negocio local


