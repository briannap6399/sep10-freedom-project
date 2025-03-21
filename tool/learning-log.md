# Tool Learning Log

## Tool: **Animate CSS**

---

### Date 3/7/25:
#### I had discovered how to Repeat & Speed-Up/Slow Down Animations.

I started my journey by looking through the main webpage of [Animate CSS](https://animate.style/), before scrolling down to the tabs about **Utility Classes.** I then noticed the base CSS for the **Slower, Slow, Fast & Faster Classes**, which as the title implies, speeds up or slows down the animation of your CSS, and I got curious about them, because I believe the class could work well with my main idea for my final website. I decided to test the classes, mainly by going to [My Animate CSS Tinkering File](animate-css-tinkering.html) and considering what would have happened if I were to use it on a sample of HTML, as presented here:

```HTML
<style>
h1 {
  color: purple;
  display: inline-block;
}
</style>
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css"/>
</head>
<html>
  <body>
    <h1 class="animate__animated animate__bounce animate__repeat-3 animate__fast">Presto! One Animated object.</h1>
  </body>
</html>
```
At first, I was confused why it wasn't working whatsoever, however I had to double check the webpage, only to realize that the prefix you need in order to work these classes required **2** underscores, instead of 1. I need to keep that in mind as I get closer and closer to the final project, mainly because I have a feeling that this type of simple accident will repeat itself. Anyways, when I noticed that the CSS made the Heading go faster, I decided to scroll down further, mainly to see if I could try and learn any other classes. That was when I stumbled upon **Repeating Classes**, which simple enough, repeats the amount of time your animation happens. It could happen once, all the way to it be infinite.
  * Please note that when you're making your CSS repeat infinitly, there won't be a special property, compared to other sets.

Similarly to the Speed Up and Slow Down Classes, you have to be mindful that you need **2** Underscores. This not only applies to this, but to other portions as well. But anyways, I decided to try it using some HTML, specifically the one I had previously set up to try the Speeding Up and Slowing Down Classes, and added in a class that would make the animation repeat 3 times. (I honestly wanted to see the class more effectively, but not last infinitly, hence why I chose for it to repeat only 3 times) The End Result is what I showed with the HTML above, but I honestly really like how it came out.

### Date 3/14/25:
#### I had further comprehended the animation classes.

For this week's learning log, I decided too not dive my feet out so deep, and instead, planned on taking it easy, opting to only check out more animation classes. The Category that has interested me the most would absolutely be what I call the ***'Rotation Classes'.*** These classes, as the name implies, rotates. These Classes are split into 2 Variations, which in this case, I'll refer to them as Sub-Classes: Entrances and Exits. I'm more so interested with the Exit Sub-Classes, as the way they are animated is more closely tied to what I had envisioned in my head for the 2-D 'Pen Animation'. Maybe if I can group the psrts of the pen together whilist having every part that makes it up animate, it'll look like a Word Cloud? I'm a little unsure, but from what I tried, it seems like a huge possibility.

```HTML
<h1 class="animate__animated animate__animate__rotateOutDownRight">Test Sample</h1>
```

Only the future really knows if it'll work, but I have high hopes.

<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
