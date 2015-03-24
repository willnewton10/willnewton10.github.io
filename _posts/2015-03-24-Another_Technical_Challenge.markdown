---
layout: post
title:  "Another Technical Challenge"
date:   2015-03-24 9:58:00

---
####TL;DR
* Did a technical challenge yesterday, 
* was dissatisfied with my code, 
* so I [rewrote it and put it on GitHub][github].

Yesterday, I went in for a technical challenge for a company I want to work for. 

I'm not going to name them, because if I did, then potential interviewers might be able to use Google to gain an unfair advantage for their technical challenge. Then they would be forced to invent new challenge-scenarios.

They gave me 3 challenge-scenarios to pick from. I had one hour. I had to use java. There was no internet connection (intentionally) and they supplied javadocs as local html files.

The 3 challenges were:

 1. make a program that uses a cipher-key to encipher and decipher text
 2. make a some sort of server that provides a key-value store that you can read from, add to, and delete elements from.
 3. make a program that mimics the game Battleship.

I chose the first and to save time, I didn't even look at the specs provided for the other 2.

The man facilitating did a good job of clearly explaining things and showing me the set-up.

I has a linux laptop. Each scenario had a spec as well as some scripts to help build and test it.

It did not have emacs, which is what I use these days. So I used Gedit. That slowed me down a bit.

At the start, I was typing stuff and running the build scripts but my changes weren't showing up. I had a moment of panic. _What the hell is going on???_ But it was because the keys on the keyboard were backwards from what I was used to: `Ctrl` and `Fn`. So, for example, I `Ctrl+S` was not saving.

As usual, I was _flooded with adrenaline_, because that's what happens to me in situations where the purpose is to evaluate me. I had the whole racing-mind thing happen again, where I can't really think all that clearly. I ended up deciding to "just make something that works" before the end of the hour. Make it work first, then make it nice. Unfortunately, I ran out of time, so I failed to make it nice.

And It was not nice at all! One bad decision I made was to use a `Map<Integer, Integer>` when I should have made a `Map<Character, Character>`. So I had a few lines of really unnecessary casts when I could have just let java do its natural "boxing" and "unboxing."

I have also never made a java program that could take text from standard input. For example, piped from an echo command. 

 * `echo "some text" | java TheProgram arg1`

Was a bit thrown off by that. But you can use `System.in` and just in the ints, casting them to chars, until you reach `-1`. In my solution I used a `Scanner`, wrapping up `System.in` but, from checking it out afterwards, I think `Scanner`'s `next()` method ignores whitespace. This didn't invalidate my solution, but that was just luck.

Anyway, I was itching to improve my crappy adrenaline-fueled solution, so I re-did it and put it on GitHub. You can [check it out][github] if you want, but it's probably boring.

By running out of time, I also missed my chance to tackle the bonus-problem. The enciphering process ignored space characters. So the bonus challenge was: given some text that was enciphered and then deciphered, make a program that tries to guess where the spaces were. A text file with words is provided. It also gave the hint to go for larger words first. 

I have thought of solutions for this, but I have not yet thought of a _good_ solution, due to its combinatorial nature.

[github]:     https://github.com/willnewton10/interview-1