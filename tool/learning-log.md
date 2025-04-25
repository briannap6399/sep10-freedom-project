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

### Date 3/24/25:
#### I started including CSS Variables.

Before I truly go into the log, just want to apologize for not having a log for last week. There was a project, and I believed that the project had priority over the Learning Log, to the point where last week would be skipped.

Anyways, I had started to dabble                                                                                                                                                                                                                          into the usage of what's known as _Custom CSS_, which are basically unique Variables designed to be used with CSS. From what I've gathered from Animate CSS, I realized that there are **3** Primary Variables in which I can use; `--animate-delay`, `--animate-duration`, and `--animate-repeat`. What I find interesting from these Variables is that it takes the already set up classes you have, and basically can extend or even shorten their animation status. For Example, let's say I have this line of code:

```HTML
<style>
.animate__jackInTheBox {
  color: blue;
  margin: 50px;
  --animate-repeat: 4;
}
</style>
<body>
<h1 class="animate__animated animate__jackInTheBox animate__repeat-3">Key Demo.</h1>
</body>
```
Notice how I gave the Jack-in-the-Box Animation a repeating cycle of **3**, but upon using CSS, I gave it a repeating variable of **4**. What do you predict would happen? Admittedly, I thought that the animation cycle would only repeat itself **7** times, with the 4 established from the CSS Variable adding onto the 3 established from the Class. However upon previewing the CSS, it did not repeat 7 Times. Instead, it'd repeat **12** Times. This is because of the fact that the cycle of animation itself is being multiplied by the requested amount through the Variable. As we all should especially know by now, 4 times 3 is 12, hence the 12 Repeation. But does this apply to the other Variables as well? Somewhat. Let me use the `--animate-duration` Variable for example. For it. my code will look like this:

```HTML
<style>
.animate__jackInTheBox {
  color: blue;
  margin: 50px;
  --animate-repeat: 4;
  --animate-duration: 900ms;
}
</style>
<body>
<h1 class="animate__animated animate__jackInTheBox animate__slow animate__repeat-3">Yet another Demo.</h1>
</body>
```
Because the Variable itself sets the animation to last for about **900 Milliseconds**, despite the fact the the code has a class that makes the animation slower than usual, the animation itself will be a little quick regardless, and I find that fascinating.

### Date: 4/5/25
#### Keyframes (Week 1)

I think this might be the first time I try to do several weeks on the same topic. This might sound counterintutitive, especially since this log is supposed to be designed to include several unique topics, but, and this is for me personally, I find myself struggling with Keyframes, and understanding how to use them. They remind me a lot of some of the code I'd see in an animation in Scratch, but of course without the `If Start is Pressed` sequence of code. Anyways, for this week, I tried to understand the structure of a Keyframe. (As in, try to understand how it's code should look) As of right now, I have this:

```HTML
<style>
@keyframes none{
  0% {color:red;}
  50% {color:green;}
  100%{color:blue;}
}
</style>
```
I was given advice from a friend that the name I select to be used for the keyframe needs to match in a specific way, however, I'm not certain on how I can name the keyframe. I did use [this Animation Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-name) as a sort of guide, and from what I can understand, I need to give one portion of CSS `animation-name: [Insert Name];`, though when I tried to plug in the name `none`, which was an example featured on the Guide, I didn't get a reaction from the CSS. Maybe it's because the sequence of code it's attached to is already being animated by Animate CSS? Whatever the case, my main goal right now is to try and get it to work. I plan on looking at more Guides, and even doing some Youtube Researching in order to find out what I can do in order to make this more active. But going back to the guide, apparently the 'hover' part of a button or image for example can actually be animated, which does make me curious; What if I tried to replicate it's effects in what I'm calling the ['Tinker Pad'?](animate-css-thinkering.html) It would make for good practice that's for sure.

<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
