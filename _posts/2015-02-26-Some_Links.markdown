---
layout: post
title:  "Some Links"
date:   2015-02-12 14:59:44

---

To start of this blog, I will post some links.

I had a programming blog before but I didn't really use it very often. The most interesting thing there is probably the ["nav-mesh" I made with JavaScript][navmesh]. It takes a set of polygons and computes shortest paths from one vertex to another. It was fun to make because I got to think about computational geometry. For example, the typical shortest path algorithm does not move *accross* polygons, so made an algorithm to generate a "visibility matrix": the graph that describes which nodes can "see" other nodes. (If the polygons are walls and the nodes are their corners, can one corner "see" another corner?) My algorithm for creating this visibility matrix was O(mn^2), where n is the number of nodes (corners) and m is the number of edges (walls): for every pair of nodes, check if the line they make intersects with a wall. I didn't like this runtime, but because it was just for fun and because I was inventing it, that's okay. I guess I made that quite a while ago.

As you can probably tell from the address of this blog, it is hosted using github. So far on [my github page][github], all I have is a little [just-for-fun project][gh-node-algs], where I'm implementing classic data structures and algorithms with node.js. 
I also have a [thing I've recently hacked together][gh-tpl-reviews] with JavaScript. It's an application that lets a user search the Toronto Public Library for books and then it will also search Amazon for the corresponding reviews for those books. I'm using Open Shift and their cloud to host it for free. You can [try it out for yourself][rhc-tpl]. 

Some other things I've been doing lately:

* I have been doing the 'training pages' over at [usaco][usaco]. This site attempts to teach programmers techniques for programming competitions like IOI and TopCoder. They only accept C, C++, Java, and Pascal, so I have been re-visiting Java a bit. I've joined in at [Code Forces][code-forces] a little bit lately. My skill level there does not satisfy me! The same can be said for my [TopCoder skill level][topcoder-profile].
* I found a book at the Toronto Library called "How to think about algorithms" by [Jeff Edmonds][jeff-edmonds]. It turns out, he's a teacher at York University (which is not too far away from me, as it is in, or at least near to, Toronto). He has a page online with [video lectures][jeff-edmonds-videos] for an algorithms course based on this book. "How to think about algorithms" is the perfect title for this book.
* I have been teaching my cousin's son how to program. We have been using a site called [RexTester][rex-t], which allows people to collaborate on executable code in real-time. We're using Python. He lives in Finland, so that's why we need something like RexTester. I have another friend who was semi-interested in learning to program, for the purspose of making games. With all of these people wanting to program, I ended up writing a [blog post intended for absolute beginners][how-to-prog]. I'm not sure if I was successful and never showed it to either of those two people! I think that is because I am very conscious of how the number one obstacle to absolute beginners is _being overwhelmed by information_. Sometimes, when you are teaching someone, the best thing to do is to be quiet for a second and let things you've already said sink in to their brains. Pause with the flood of information.


[github]:      https://github.com/willnewton10
[navmesh]:     http://willsprogramming.blogspot.ca/2013/05/navmesh-newer-wait-few-seconds-for-it.html
[gh-node-algs]:    https://github.com/willnewton10/node-algs
[gh-tpl-reviews]:  https://github.com/willnewton10/tpl-reviews
[rhc-tpl]:     http://tpl-wn10.rhcloud.com/
[usaco]:       http://www.usaco.org/
[jeff-edmonds]:    http://www.eecs.yorku.ca/~jeff/courses/3101/syllabus/
[jeff-edmonds-videos]:   http://www.eecs.yorku.ca/~jeff/courses/3101/ass/video.html
[how-to-prog]:   http://willsprogramming.blogspot.ca/2015/01/learning-to-program-for-absolute.html
[code-forces]: http://codeforces.com/profile/WillNewton10
[topcoder-profile]:  https://www.topcoder.com/tc?module=MemberProfile&cr=23157788
[rex-t]: http://rextester.com/
