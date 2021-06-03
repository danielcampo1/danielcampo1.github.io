---
layout: post
title:      "React project"
date:       2021-06-03 21:23:13 +0000
permalink:  react_project
---

Could this be the final Module from school?

This is my last module at Flatiron school.

In the last 10 months we have learned multiple languages to get us to the point we are now, And with this finally project focused around reactJS/Redux. I have felt like I have learned so much but it also feels like I barely know anything, maybe that’s my imposter syndrome I hear everybody talk about. 

The biggest thing thing that took me a while to understand was the Reducer, Action, state combo. I think its because the wording just doesn’t make since with me but the more I used it I began to understand its flow. A huge contributor to making the these things run in a circle are the connect() and Provider imports from React Redux middleware. Provider makes sure that my React app can access data from the store that got created, and connect() allows whichever component to specify which state and actions the app needs access to. 

￼

An example of my actions would be the getPlan() asynchronously fetches from my back-end routes, and dispatch a reducer a value

￼

The dispatch is sent over to match the type statement, which in this example “FETCH_PLAN_SUCCESS” is matched up to return back the payload or data from the actions fetch request. And in the end should be updating and creating a new state.

Yes this is a very broad understanding of this but I felt like this was such a big thing for me to finally understand and took me lots of debuggers and pry’s in the backing to start understand the flow on where everything is going. By no means is this project complete or even fully functional but I feel proud that I created something and actually understand what’s happening inside. Still have lots to learn and I hope this isn’t my final project and I continue and find my Web Dev job.
