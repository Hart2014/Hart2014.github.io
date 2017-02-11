---
layout: post
title: BlocFlix
thumbnail-path: "img/blocflix.png"
short-description: BlocJams is an online music player that allows you to stream music.

---

{:.center}
![]({{ site.baseurl }}/img/blocflix.png)

## Explanation

Bloc Jams presented a nunber of challenges along the way, which each caused moments of analysis and research. One in particular, was rather difficult in finding. This ended up being an error with albums displaying.

## Problem

In the colleciton menu, users have the option to select the album which they would like to listen to. Once they click on that album, they navigate to the album page, where the individual songs are displayed. Users can then click on those tracks to play them, but in this case, those songs were not displaying. Everything else from the album would display but the songs. 

## Solution

The first solution was to check the console in Chrome developer tools. This usually yields some sort of lead that you can follow. Unfortunately, this went no where. The second solution was then to identify the source of where the problem came from, starting with how songs were instantiated. After combing through the code, I realized that I had mispelled and album reference in a jQuery reference, which prevented the songs from displaying.

## Results

After correcitng the spelling of the word "album", the songs appeared again!

## Conclusion

Make sure that you take time writing your code. An ounce of prevention is worth a pound of cure. 