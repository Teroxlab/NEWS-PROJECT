# NEWS-PROJECT
AET
This project is a web development exercise.

Goal
You are going to make modifications to a webapp using the Polymer 2 library around the WebComponents.

This application displays articles retrieved from NewsAPI , which aggregates several news sources. It will also filter the content displayed.

The targeted browsers are the latest versions of Firefox, Chromium and Edge.

Method of working
The code is versioned on git. You will respect the following practices:

you work in a separate branch of master

your commits are simple (maximum functionality) and documented in English

The tasks are quite independent, deal with them at your own pace.

If you are feeling creative, feel free to go beyond exercise (but always stick to the specifications given).

Prerequisites
Set up a working environment for Polymer:

install nodejsand npmon the machine

install bowerand polymer-cli:npm install -g bower polymer-cli

Preparation
Clone this git repository and explore the files

To install the project dependencies, run the command bower installin the project folder

To test the application locally, run the command polymer serve

Exercises
Editing the item news-card
The element news-carddisplays a news, composed of a title, its author, an image, a publication date, a description and a link to the article.

Navigate to the demo url (ex .: http://127.0.0.1:port_number/src/news-card/demo/index.html )

Add the following properties to the element: title, author, description, imgand hrefa String and publishedAttype Date.

Edit the element template and add styling to match the spec cf img.

Convert the date to a readable English format.

We would like the description to be revealed when hovering over the image, over it, make the necessary changes.

Add to the image, a placeholder of your choice in base64.

When clicking on the element, the link should open in a new tab.

Increase the shadow around the element when the cursor is over it.

Optional - You can modify the item's demo news-cardto fetch data from file data.jsonusing the Fetch API. In the demo file news-card/demo/index.html, listen to the event WebComponentsReadyon the document, then retrieve the contents of the file data.json, select the element news-cardand populate it with this data.

Data recovery from NewsAPI
Create a new API key at https://newsapi.org/ and configure the item <news-list>in search-new-app/search-new-app.html.

Navigate to the url of the application served by the command polymer serve.

Create a new element <news-list>which takes as input the id of a source and an API key.

it uses the item iron-ajaxto generate a query that retrieves articles when the source changes.
it maintains a property newssaving the content of the last request.
it iterates over the news to display them with <news-card>.
