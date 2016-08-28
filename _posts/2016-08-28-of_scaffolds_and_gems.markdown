---
layout: post
title:  "Of Scaffolds and Gems"
date:   2016-08-28 17:03:44 +0000
---

Throughout my coding journey I have reached various milestones; [my first computer program](http://http://yechiel.me/2016/08/08/program_0/), [my first published gem](https://rubygems.org/gems/dansdeals), and my first fully functioning bot capable of playing [Tic Tac Toe](http://yechiel.me/2016/08/26/tic_tac_tips/).

Recently I reached another milestone. My first contribution to an open source project was accepted and published. I guess I managed to convince someone else that I know how to code as well :)

It all started when I finished the section on Sinatra in [Learn](http://learn.co/with/achasveachas)'s curriculum. At the end of the section we are expected to build our own Sinatra app from scratch. I have [blogged](http://http://yechiel.me/2016/06/26/gem_instal_swim/) in past about how sometimes being thrown into the deep-end is the best way to learn how to swim, and somehow this time it felt a little less scary.

The hardest part of every project is to take the first step, and here too I was at a loss how to go about it. Throughout the curriculum we pass different labs and challenges, and what all of them have in common is that the basic structure for the app is provided for us. This time I was staring at a blank screen not knowing where to start.

Back when I was making my CLI gem, I learned there was a powerful tool for generating the basic structure of a gem called Bundler, if I could just find something similar for Sinatra apps I would be well on my way.

Naturally I turned to my trusted mentor, Google. 

![](http://i68.tinypic.com/23uar85.gif)

This time however Google wasn't much help. It didn't look like there was such a thing. 

So I dug around a bit more, asked around on Learn's Slack channel and found that our very own [Brian Emory](http://http://www.brianemory.com/), a fellow Learn graduate, created just what I was looking for, a nifty gem called [Corneal](https://rubygems.org/gems/corneal) that generates the basic structure for a Sinatra app.

![](https://d262ilb51hltx0.cloudfront.net/max/1200/1*UyGyw4z4YlRptP3KtY8xCA.png)

So I spent some time playing around with Sinatra, getting utterly impressed that this was all made by a fellow student, and then that got me thinking; if a fellow student made such a cool gem, knowing not much more than what I did, what would stop me from adding improvements to the gem?

There was a feature in the gem (added by another fellow Learner) that added Ruby Models to the app, I decided to take it a step further and add a feature that would add the Model along with its associated erb views and Sinatra controllers, similar, as I would later learn, to Rails' Scaffold generator.

It took 2 all-nighters during which I delved into Thor documentation, collaborated with a fellow Learner in Nigeria, and spent hours getting frustrated by a bug in our IDE, but finally my feature was ready. I submitted the pull request and not long after was notified that my feature was accepted!

![](http://i63.tinypic.com/qp1bvn.jpg)

My first reaction was severe impostor syndrome "Oh my gosh! He published it! What will happen when everyone will realize I had no clue what I was doing and the whole thing crashes?!" but eventually I realized that that was all part of the process, it's all part of the learning and the more real world experience I would be gaining, the closer I would get to the day when I was creating stuff all on my own!

Happy coding guys!


