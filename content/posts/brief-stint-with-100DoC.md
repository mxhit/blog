---
title: "Brief Stint with the #100DaysOfCode Challenge"
date: 2021-11-17T19:30:48+05:30
draft: false
---
The easiest part about the #100DaysOfCode Challenge is taking up the challenge. The harder part is committing to it while coming up with new ideas for each day; it’s both exciting and daunting. I experienced this for the first time when I publicly committed to the challenge on Twitter. It is generally advised to have a rough map of ideas ready when taking up the challenge but I took a different approach of establishing rules simply because I need to fall in line with them while developing things every day. My rationale at the time was:
> Define concrete rules and stick to them while thinking of ideas that fall within the rules.
---
## Day 1: Designing the book cover of “Do The Work” by Steven Pressfield

So when it came to deciding the task for Day 1, I found myself extremely unprepared. After spending a better part of an hour brainstorming, I thought of a book that I had re-read a couple of days ago. The book was Steven Pressfield’s Do The Work, and it has been of immense value to me. Just before taking up this challenge I had developed my portfolio website using React, and it would not have been possible without the help of this book. You see, I had been trying to develop this website for the last two years — using vanilla HTML and CSS, JSP, and Angular.js — but I would drop it as soon as I came across some form of a problem — ‘Resistance’ is the term the author uses in this book. The concepts the author covers in this book really helped me understand the forces at play when it comes to doing any type of work. So, when I found myself struggling to come up with an idea, I thought of designing the book cover using CSS. I was and still am terrified of doing CSS art but a fellow friend on Twitter managed to convince me to do it.

Now that I had an idea ready, it was time to put it into action. The HTML part was very straightforward and I was done within a few minutes. The CSS part, however, still intimidated me. I was able to manage the styling of text elements without breaking any sweat but the thought of designing the pencil using CSS kept me terrified until I actually started working on it.

### Crafting the pencil

Despite being terrified, I stuck to the basic fundamentals of problem solving and divided the problem at hand into smaller problems. The basic skeletal idea I had looked like this.

```html
<div id=”pencil”>
   <div id=”eraser”></div>
   <div id=”holder”></div>
   <div id=”wood”></div>
   <div id=”tip”></div>
</div>
```

I immediately started working on each component of the pencil starting from the eraser as it was the easiest component and I knew I would be needing some confidence when moving to the other components. Everything went well with the Eraser and I completed the Holder and the Wood components relatively quickly.

What I did not account for in the skeleton of the pencil was the triangular design you get after sharpening a pencil. This meant I had to refactor the HTML code to accommodate it and then design it as well. I had to look up “how to make a triangle using CSS” to get this done. This also helped me with finishing the tip of the pencil and adding the black nib at the end.

The final pencil code looked like this.

```html
<div id=”pencil”>
   <div id=”eraser”></div>
   <div id=”holder”></div>
   <div id=”wood”></div>
   <div id=”design”>
      <div id=”sharpener”></div>
      <div id=”sharpener”></div>
   </div>
   <div id=”tip”></div>
   <div id=”nib”></div>
</div>
```

[Here is my Codepen for the book cover.](https://codepen.io/mxhit/pen/jOweZgY)

### Takeaways

I spent more than two and a half hours on this and I learnt about a lot of concepts I need to focus on:
- Master basic shapes using CSS before making moving to complex shapes.
- I need to practice positioning and aligning elements.

### Approach going forward

I have realised I have little to no knowledge about CSS that is required for diving into CSS Art, and I need to practice CSS as much as I can before diving into complex CSS art.

---
## Day 2: F1 gantry lights

I decided on the F1 gantry lights primarily based on the takeaways from Day 1; secondary reason is my love for Formula One but we can ignore that. Now, I had to keep it simple and ensure I work on basic shapes. For those of you who do not know what gantry lights are, they are basically used to indicate the start of a race — they have some other purposes as well but it is irrelevant at the moment.

A couple of [rectangles with a few circles in them](https://media.gettyimages.com/photos/the-start-lights-taken-during-the-canadian-formula-one-grand-prix-on-picture-id2091554?s=612x612), yeah. You can see why this seemed like a good choice for creating basic shapes with CSS. The skeletal structure also seemed to very simple for this one.

```html
<div class=”f1-lights”> <!-— one vertical light column -->
   <div class=”stand”></div> <!— horizontal bar connecting all vertical columns -->
   <div class=”light-strip”> <!— vertical strip containing lights -->
     <div class=”light”></div>
     <div class=”light”></div>
     <div class=”light”></div>
     <div class=”light on”></div>
   </div>
</div>
```

Rest of the process was fairly simple, and I was done with it in an hour before the start of the Russian Grand Prix. This was fun and I feel very confident for tomorrow.

[Here's the Codepen.](https://codepen.io/mxhit/pen/ZEymGrX)

### Takeaways

- Basic shapes are not very complicated and I will probably work on them on the side instead of reserving an entire day of the challenge for them.
- This would have seemed a lot cooler if I knew how animations work in CSS. Time to get on it.
- Need to learn how to blend colours in CSS.

---
I quit the challenge a few days after Day 2 as I was unable to dedicate time to the challenge. Simply put, the challenge ranked way lower in my list of priorities to be worth spending time on. I could definitely see the merits of undertaking this challenge as it forces you to choose a specific topic to learn and acts as a catalyst in the learning journey.

I would recommend this challenge to anyone who can spare a good amount of time on a daily basis for this challenge.
