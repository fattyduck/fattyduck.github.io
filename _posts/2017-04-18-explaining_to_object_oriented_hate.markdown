---
layout: post
title:  "Explaining the Object Oriented Hate"
date:   2017-04-18 08:56:32 -0400
---

Assuming I am not the only one who googles randomly about programming paradigms, many have seen the intense hate Functional developers seem to hold for Object Oriented programming. Before continuing, I would like to share two very important facts. Probably the most famous quote used by Functional developers was "You wanted a banana but what you got was a gorilla holding the banana and the entire jungle." by Joe Armstrong. The most popular programmer joke would probably be the optimst, the pessimist, and the programmer vs half glass of water. The programmers responce was the glass is twice as big as it needs to be. 

From the facts above, we can conclude programmers dislike wasteful behaviors and Functional programmers see Object Oriented progamming encourages wasteful behavior. Along with my random googling about programming paradigms, I also like to randomly browse through github to look at code. To be honest, from browsing github I have never found code wasted at all. So where, do Functional Programmers get this idea? The answer is very simple, personal experience. 

Fact is, the most popular programming paradigm today is Object Oriented programming. couple years ago, Object Orient programming was also the most popular programming paradigm but with a wider margin than ever. By the law of averages, a lot Functional programmers now were Object Oriented developers. By the law of averages, the now Functional programmers has worked with a lot of Object Oriented developers. Also by the law of averages, Object Oriented paradigm holds the greatest number of beginner developers. 

My personal experience with a developer in an Android project. This developer thought it would be a great idea to split Traffic Tickets model into Traffic Tickets, Traffic Violations, and State Law Violated. We pulled from API and only presented Traffic Tickets to users with the name property from Traffic Violations. Basically we spent time and computer resources parsing and populating two models whose sole purpose was to take up space from database and waste time. 

From a business point of view, imagine an aspiring educator whose goal in life was to make schools for the underpriviledged. The school has just been created, he spends the next 3 years planning incase one of his students was an evil genius. I think the biggest issue is certain people don't understand planning at all. By writing code core to functionality, in the future, if I need new functions, I will write the code. By writing future might be implemented code, I might spend the future deleting or changing most of the pre-written code. 
