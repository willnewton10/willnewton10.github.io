---
layout: post
title:  "Sequel to Amazon Technical Interview"
date:   2015-03-13 20:56:00

---

So, surprisingly enough, I did get called back for an on-site interview with Amazon. (However, there are some complications which I will discuss in a later post.)

I was quite surprised to be called back. My girlfriend says I _underestimate myself_, but a friend of mine says I _overestimate my competitors_. Those two possibilities are not necessarily mutually exclusive.

One of the main reasons I decided to change jobs was to find a place where I could work with and learn from multiple smart programmers. This does not necessarily mean that they _teach_ me things; it may just mean that they say "no, think about this other way of doing _x_." In other words, the minimum I need is for someone to point at something and tell me something constructive and then the rest is up to me to research whatever it is. 

If we think about this as a search problem, we can think about it like the difference between something like BFS/DFS and A*-Search. When I am developing alone, I will pick the solution that I think is worth trying, try it out, and then backtrack and try some other solution. But, in reality, the time constraints can make it impossible for a _good_ solution to be found this way. If I have someone who has more experience than me, they have more information about the search-space, and their accumulated knowledge can act like a heuristic that says (while pointing somewhere), "_this_  would the best direction for you to go in right now."

For those of you who want me to explain this without the jargon, imagine I am an ememy in a video game and that by catching the hero, I find my solution. Without more experienced people over-looking, it is as if I am blind and I have to walk around the map, _trying possible solutions_, without even knowing the general direction of the hero I am chasing. With an experienced person to give feedback, they can say:

 * "move _that way_, because he's over there" or 
 * "move _this other way_ because there is a huge wall blocking you." 

There is also the problem of _knowing when you're right_. For a given problem, there are many solutions, but they can differ in quality. Without an experienced onlooker giving feedback, you could find a local maxima, but fail to even come close to the global maxima, because you don't have that perspective. So, with some design I've thought up, I could do the best possible _with that design_, but if I was working with some other better design, I could make something even better.

Hm. What could be a classic and humourous example of a person mistaking a local maxima for a global one?

Anyway, one of the things that was really cool about the Amazon Technical interview is that in about an hour, I experienced this phenomena of someone more experienced pointing some things out to me. Here are some of the things that I have learned, either during the interview or catalyzed by it:

* binary search trees are cool, and I think _balanced_ BSTs are even cooler.
    * you can quickly find minimums, maximums and next-highest / next-lowest values (`O(log n)`)
    * you can find ranges quite fast
    * you can use them for sets or key-value mappings
    * they can use less space than hash tables
    * they avoid the hash table problem of re-hashing (when you need to expand your underlying array)
    * they avoid the hash table problem of worst-case search, when everything in the hash table maps to the same spot

* the `List<T>` type in Java is not an abstract class. It is an interface.
    * this makes sense, because thinking about an `ArrayList` and a `LinkedList`, there is very little functionaliy that could be abstracted out to a base class.

* When would you want to use an abstract class over an interface?
    * One way to look at this question is as a trick question. You can use both. The interface can be used as an interface and the abstract class can be used as a partial implementation for that interface. So the difference between an abstract class and an interface is largely the difference between a class and an interface; one is an implmentation and the other is an API.














