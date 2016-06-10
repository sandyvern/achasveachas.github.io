---
layout: post
title:  "puts #{solution}"
date:   2016-06-09 22:29:10 -0400
---


 So last night I had an epiphany. It's the kind of inspiration that only comes at 3 am when the house is quiet and your head is about to explode from a night of writing (and rewriting) code.
 
 For 2 nights I've been up cracking my head trying to write a working method. I am in middle of writing a game of Tic-Tac-Toe, where you can play against the computer. Obviously, in order to ensure my game isn't **completely** boring I need my intelligent computer player to have some level of strategy.
 
 So I've been pulling all-nighters trying to code this one method that would let the computer figure out if a corner was taken, and if so to take the opposite corner and hopefully make (or block the other player from making) a fork. The problem was that no matter how much I iterated and looped, returned values and assigned variables, the computer refused to do what I wanted it to do.
 
 Then finally last night, at that magical hour between night and day, just as I was about to throw the monitor out in frustration, the solution hit me. A solution so simple I refused to think of it initially, but once I accepted it taught me something profound (or so I think, this may well be my undoing as programmer some day).
 
 So are you ready for it? Here goes:
 
```
  def opposite_corner
    case
      when board.taken?(1) && !board.taken?(9)
        9
      when board.taken?(9) && !board.taken?(1)
        1
      when board.taken?(3) && !board.taken?(7)
        7
      when board.taken?(7) && !board.taken?(3)
        3
    end
  end
```

 (In english what this means is simply: if the top right corner is taken and the bottom left one is free go there. If the top left is taken and the bottom right is free take that one, and so on for all 4 corners)

 The actual thought that blew me was this: here I’m breaking my head trying to automate a method to do something, but why? There are exactly 4 possible moves. Is it really worth the headaches, frustration, all-nighters, and sleepy workdays? Not to mention all the cups of Starbucks I needed just to get through the day? All just so I can automate a process that I could easily do manually, and probably in less lines of code?
 
 Sure we programmers are lazy, and if we can automate something we don’t like to do it manually. I have to admit, I’m still not as happy with my code as I probably would have been had I figured out a more elegant solution. Nevertheless, I believe once in a while we have to know when to step back, when to say “listen, you are overcomplicating this, do it simply and then go get some sleep!”
 
 
 
 ![](https://imgs.xkcd.com/comics/the_general_problem.png)
(Credit: [XKCD](https://xkcd.com/974/))


P.S. If anyone is interested, the project can be found [here](https://github.com/achasveachas/ttt-with-ai-project-v-000), If anyone has any suggestions on how it can be improved, especially the #opposite_corner method in the article, I would be extremely thankful.

