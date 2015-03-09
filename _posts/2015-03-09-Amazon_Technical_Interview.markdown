---
layout: post
title:  "Amazon Technical Interview"
date:   2015-03-09 14:59:44

---


This morning, I had a technical interview with a real-life Amazon software developer. It was about an hour and ten minutes. I don't think I failed _too_ miserably but I did not do as well as I wanted. The man who was conducting the interview was really friendly and supportive which I really appreciated. I get terribly stressed in interviews (and I lose lots of energy _before_ the interview, thinking about what might happen). I start talking too fast and then I ramble on and on. So it helps when the person on the other end is kind.

Let's go over some of the blunders I made:

* First of all, I don't express myself well when I am flooded with adrenaline, so a lot of stuff I said probably sounded incredibly _awkward_. Then, afterwards, for each memory, I deal with one of two cases. The first case is that I remember what I said and then my thoughts are along the lines of "man, I really should have said <something-else>!" In the second case, where I don't remember what I said, I can let my paranoid imagination take over and make up something really embarrassing, in which case I think "OMG, I didn't say _that_, did I?" This really happens.

* I couldn't tell him the difference between an abstract class and an interface. (You can put functionality into an abstract class.) Last time I used an abstract class was back in second year at George Brown, so I forgive myself for not knowing this. Plus, I think in interfaces, not with abstract classes. But... you can give all of the excuses you want. Can't change the past!

* I may have given the definition for a Binary Tree when I was asked what a "tree" is. I don't remember if he said "binary" or not. I definitely described a binary tree.

* May have had some other blunders, early on, but I don't remember because of the adrenaline. (My best way of dealing with this is trying to breathe slowly and steadily, but if anyone else has any techniques, I would appreciate hearing them.)

* In the specific problem that we were going over, I provided a solution involving a hash table idea. When prompted for something more efficient, and even when provided non-subtle hints, I failed to say, "oh, a binary tree." This disappoints me too, but at least I learned something valuable: in short, that trees are really cool and useful and I should give them more credit and not automatically reach for a hash table. 

* I was not fast enough with run-time calculations. He asked me what the worst-case scenario would be for this hash-table-style solution. He kindly gave some hints about hash tables as I tried to remember. Essentially, the problem was: you are reading an array of `n` elements and counting the frequency of the values you come across. I was storing the counts in a hash table, where the key is the element from the array and the value is the count--that element's frequency. The worst case is that all of the values hash to the same index in the array. To examine all elements in this linked list (which is located at that index in the array), we require `O(n)` time. (For the binary tree alternative mentioned above, the worst case for a lookup is `O(log n)`, although I think this may require a "balanced" binary tree. With a normal binary tree, I think the worst case be `O(n)` for a lookup, if the tree has 1 really long branch. I guess review is required.)

* I kind of don't want to fully remember this last blunder. I was trying to call my girlfriend after the interview was over, but I think I redialed the interviewer's number. I believe I hung up after 1 ring. _Embarassing!_ I'm not completely sure that this happened, and I kind of don't want to look at the phone's history to find out. 

Why did I (maybe) accidentally call him back? It's because I was using a different phone. This was a phone interview, where I would also have to code. So I required a way to have my hands free. My phone, being an old, clunky flip-phone, does not have a headphone jack and I was not confident enough with the speakerphone to use it. So I needed to borrow someone's phone or buy a new one. I'm going to skip details about why I did not want to buy a new phone. 

The solution I came up with, along with my awesome girlfriend, was to just trade phones with her, but also _switch SD cards_. So, with her smartphone, I could easily use headphones and she could still have a productive day at work. I thought it was really sneaky for us to switch cards like that. The only downsides are: my flip phone is slower to text with (which may slow her down at work) and I kept hearing a noise every time she receives an email. (We are both under the same phone company, so, as far as I know, that is what allows us to switch cards.)

If I had to guess whether or not Amazon is going to call me back, I would guess that they won't. I honestly have no idea, but I don't think my Data Structures / Algorithms / Object Oriented Programming was up to their standards. 

If I could do it all over again, here is what I would do differently:

* I would do a more thorough review of data structures and algorithms: make sure I could describe
  *  how everything works,
  *  what the runtimes are for using the algorithm or data structure, 
  *  and why I would want to use one solution instead of another.
* I would start reviewing long before applying instead of about one week before the interview.
* I would review OOP as well and possibly design patterns. The abstract class blunder could have been mitigated this way. (And he did ask about a few design pattnerns).
* I think if I had reviewed more, I would not have been so adrenalized.

Good luck to anyone else who applies to Amazon.