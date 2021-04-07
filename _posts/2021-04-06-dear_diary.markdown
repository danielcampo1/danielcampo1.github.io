---
layout: post
title:      "Dear Diary"
date:       2021-04-07 00:51:19 +0000
permalink:  dear_diary
---


Hello fellow Developers, 

Since finishing up my Ruby on Rails project, we have immersed ourselves in JavaScript fundamentals. These fundamentals involve learning about JS events, DOM manipulations, ES6 syntax sugar, and OOJS (Object Orientation JavaScript).   I was trying to brainstorm ideas on what I wanted this Single-Page Application to do or even look like, and I really struggled to figure out what I wanted to do and what I actually had time to create. After 4 backend creations and 10 days later, I decided to finally stick with the project idea to make an app that created little journal entries. Yeah.. if it sounds basic its because it is very basic .

This app will have a Form in HTML that the user can input their journal entry with a title of their choosing to represent the overall naming of the journal they are about to write. A description box, to write however much their heart desires, and an image, since some people like to take journalling serious and add drawings or memorabilia they can take pictures from online to help tell the story of the journal entry.  Since this project requires us to have a Has_many and belongs_to relationship, I made these journals belong to a category table that were broken down into 4 categories (life, photography, real estate, and tech) just to give the app a little sense of organization.

MY FRONTEND

When I finally finished up my backend and basic structure of html and got to my frontend, it felt like I hit a wall forgetting everything on how JS worked. But watching some videos from instructors that they provided for me I felt motivated again and just refreshed honestly because I had spend the last 10 days worrying about a back end and what the project could be, and just having to remember the The three pillars of Web Programming: recognizing JS events, DOM manipulations, and communicating with the server are what make up JS.

It took me some time to understand the flow of how JS went because you have a code that runs asynchronously or synchronously. That is one thing I appreciated about Ruby on Rails, that the organization of the language just makes me all cozy inside when things have its own place for everything. But for the most part I think I was happy about the flow of my 100+ line page in my index.JS file that started from the GET fetch through my delete button on each object, to then getting the values of each input from the form, and POST fetch and showing the journal entry on the browser.  A big challenge I had was when I was refactoring and lightening up and getting rid of code to DRY it up, I started to use the Object-Oriented JavaScript for better data control. Using constructor methods and new syntax to instantiate the constructor method. But I had some problems because I used Fast JSON instead of what was taught in the curriculum which was active model JSON. Especially, when I instantiated the new method on the journal class constructor. I would call the object back after the fetch in my instantiated new for the OOJS and only get the top level info like :id, and :type. i wouldn’t be able to grab the attributes or foreign key that went along with the model to create the rest of the form. 

But soon found out that when instantiating the OOJS with fast json you need to add a second argument that gets you into the next level after the :id. By adding in the second parameter and calling, EX: Obj. Data. Attributes, and now you’ll have access to the attributes of your model. 

WHAT DID I LEARN?

Honestly, after completing the whole project I learned the most with my assessor for this module. I had the wonderful Jenn Hansen as my assessor and in my live coding assessment we took away some hard coded features and we made it more dynamic.

I had a category model, I utilized in giving some organization to the app but I ended up hard coding the categories into HTML to have one less thing to worry about but Jenn called me out and we went ahead and used it as a learning opportunity. Had to remember first this is a fetch request because we are getting information from our backend. After getting the HTTP response and converting that response to JSON and having my objects is where I struggled to do what’s next because this is where I usually googled till I got what I needed. Jenn guided me, and kept me focus on the picture of what needed to be done with out giving me the answers. 

After getting to the object of my categories model I needed to iterate over each category to display it on the DOM. So after using a ForEach on my object I queried the Document and selected the Id in my HTML that held the placement where the categories would be placed in the browser. Once the element was reached I needed to add HTML to that element by utilizing the “InnerHTML” adding the value of the drop down which was the category ID and using the name of that category to display for the user. Which created a perfectly working drop down menu, of all the categories the user can use for their journal entry. As I said earlier, I learned the most from this assessment because doing online learning you sometimes forget how resourceful a teacher can be in helping with your thought process. You could have all the information but not being able to apply it is useless. 


