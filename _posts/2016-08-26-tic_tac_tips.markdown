---
layout: post
title:  "Tic Tac Tips"
date:   2016-08-25 20:43:49 -0400
---


The other day I was helping a friend who is a little behind me on [Learn](https://learn.co/with/achasveachas
). He is trying to program a Tic Tac Toe game where you can play against a computer, and the computer wins.

The [TTT-with-AI project](https://learn.co/tracks/full-stack-web-development/object-oriented-ruby/final-projects/tic-tac-toe-with-ai) is the most challenging project up until that point in the curriculum, yet it is also one of the coolest projects throughout. It's the first time you actually create something that you can show off to non-programming friends (in fact, you can see mine [here](https://github.com/achasveachas/ttt-with-ai-project-v-000)).

Of course, you only realize the good parts after you're done, while you are working through it you only see the hard parts, so I put together a list of tips for my friend. After I sent it I realized these tips might be helpful to others out there as well. I figured I'd post the email I sent here as is. If it helped you out please let me know:

> Hey there,
> 
> Here's the list of points I wrote in my notes when I was doing the AI portion of the lab. I don’t know where you’re holding with it so some of the tips below might not apply to you anymore but they are good tips to keep in mind anways, so in no particular order:
> 
> * Have fun. This is probably the most challenging lab so far and it’s the first time you are asked to do something without clear instructions on how to do it, but the truth is, that’s how programming is done in the real world. There is no one way to solve the AI, probably every programmer who did it had his own approach and did it differently so feel free to have fun and be creative. This is also the first lab where you feel like you come out of it with something you can show and the first time you actually feel like you did something. So although it may be a tough one, it’s also the most rewarding project so far.
>  
> * Take it slow. This applies to any big problem in coding. When you start thinking of it, it sounds scary, “how in the world do you program an unbeatable AI?” So here’s the thing, don’t program an unbeatable AI, break it down to individual strategies and do one at a time. Which leads to next point:
>  
> * Make a plan. Put together a list of what it takes to win a game of TTT, starting from the most basic strategies and build your way up (can you AI recognize when it could win? Can it block its opponent from winning? Take the middle, corner, whatever your strategy is). You can check Wikipedia’s page on TTT for a basic strategy. [Here is a link to my strategy](https://github.com/achasveachas/ttt-with-ai-project-v-000/blob/master/lib/players/ai-strategy.md), I don’t think I ended up implementing all of it, do what you can and remember, it doesn’t have to be completely unbeatable, an AI that has some strategy is more than you were able to program a month ago.
>  
> * The readme part of the lab suggests a bonus project of making a “wargames” version of the game with the computer playing a hundred games against itself. I found it actually to be a great tool to check how good my AI was. It’s not so hard to implement (just make a loop that runs the game with 0 players 100 times) and I set up a counter to display at the end how many times player A won, how many times player B and how many draws, with the goal being to get it to show 100 draws every time (bonus points for fitting in as many War Games references as you can ;) ).
>  
> * Cheat. Real programming is a team effort, so while you definitely should try to figure things out on your own, once you have a method working definitely do look at other people’s code, chances are you will find someone who found a better/prettier/more efficient way of doing it (you can see other people’s solutions by going to [learn-co-students version](https://github.com/learn-co-students/ttt-with-ai-project-v-000) of the repo on github and going through the pull requests).
>  
> * Resist the need to overprogram. As programmers we want our methods to be as abstract as possible, but sometimes the more elegant solution is to just hard code a certain outcome. See [this blogpost](http://yechiel.me/2016/06/10/puts_solution/) for how I learned this lesson. 
>  
> * Infinite loops. The most common question I saw on the TTT with AI project is people running into infinite loops. In my experience it can come from one of two things a) you check and see that a spot is empty so you tell the computer to move there, the problem is when there’s a mismatch because the array stats at index[0] and you usually send your choice for a move starting at 1, when you forget to account for the mismatch you get an infinite loop where the computer tries the same move again and again and it keeps getting rejected. The second reason I can’t remember at the moment so it will be left as an exercise to the reader :)
>  
> * Remember again, the AI doesn’t have to be completely unbeatable, my AI cannot be beaten by itself and does pretty well (if not perfectly) against the human opponents I put it against. I can beat it without a problem, but that’s because I know its strategy and know how to work around it. As long as you give it some strategy you are already doing better than you were able to before you stated and you can always go back to it later.
> 
> That’s all I can think of for now, if I have anything to add I’ll let you know and as always if you need any help feel free to reach out during evening and weekend hours.

Happy coding guys!
