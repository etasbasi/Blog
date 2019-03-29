---
title: What does javascript being single threaded language mean?
layout: post
---

Contrary to most of the other popular programming languages, JavaScript is single-threaded. What this means is that the language only allows the computer to work on one operation at a time.
When JavaScript was first developed, its purpose was to allow web-sites to submit forms and do other basic functions and a single-thread language was enough to achive that functionality.

Now, each browser has a Web API, which can execute asyncronous operations like `fetch()` and `setTimeout()`. When the JavaScript engige encounteres an asyncronous code it hands it over to the Web API. The asyncronous code gets executed in the background and when it has finished executing, it gets added to the callback queue. Then, the result of the asyncronous gets pushed to the execution stack after it has finished executing the rest of the file.

Source: Udemy - Advanced JavaScript concepts, Andrei Neagoie
