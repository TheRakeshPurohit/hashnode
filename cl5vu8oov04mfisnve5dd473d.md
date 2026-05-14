---
title: "I re-wrote Array in JavaScript but as an Object"
datePublished: 2022-07-22T05:03:05.000Z
cuid: cl5vu8oov04mfisnve5dd473d
slug: i-re-wrote-array-in-javascript-but-as-an-object
canonical: https://therakeshpurohit.medium.com/i-re-wrote-array-in-javascript-daa4c564e693?source=rss-415d4a54ac94------2
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1657869124402/joBLn682d.png
tags: javascript, json, react, object-oriented, arrays

---

### I rewrote Array in JavaScript but as Object!

> [Nearly everything in JS is an object](https://towardsdatascience.com/everything-about-javascript-object-part-1-854025d71fea#:~:text=Nearly%20everything%20in%20JavaScript%20is%20an%20object%20other%20than%20six%20things%20that%20are%20not%20objects%20which%20are%20%E2%80%94%20null%2Cundefined%2C%20strings%2C%20numbers%2C%20boolean%2C%20and%20symbols.%20These%20are%20called%20primitive%20values%20or%20primitive%20types.).

Note: I could have used OOP to make the code better, reusable and robust. I was in so hurry to try out the experiment and do some code as talk is cheap. (😉)

<iframe src="https://cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Ftenor.com%2Fembed%2F12400965&amp;display_name=Tenor&amp;url=https%3A%2F%2Ftenor.com%2Fview%2Fcome-on-flash-hurry-up-ina-hurry-gif-12400965&amp;image=https%3A%2F%2Fc.tenor.com%2FhgEpIKnff6UAAAAC%2Fcome-on-flash.gif&amp;key=a19fcc184b9711e1b4764040d3dc5c07&amp;type=text%2Fhtml&amp;schema=tenor" width="600" height="400" frameborder="0" scrolling="no"><a href="https://medium.com/media/b2c482ba436e9293e797093f948a6027/href">https://medium.com/media/b2c482ba436e9293e797093f948a6027/href</a></iframe>

Well, it is true. Even \[a,r,r,a,y\] is also an object in JavaScript.

I have heard that too often. Also, I had only one inquiry. “HOW?” When I began my excursion in Javascript, I had this idea. What’s more, as I continued to learn, I discovered that inside javascript regards the Array as JSON.

I had this data for quite a while as a javascript developer. One great day, while getting back, this thought hit me (and not a vehicle 🚗), assuming somebody could get it done, Why mightn’t? Why not make an effort to execute an array in JavaScript Object all alone to perceive how it functions? It would be enjoyable. I have the beneath picture as wallpaper:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869114211/9qeh8iYpll.png)

A Richard Feynman Quote

Hold on before we go to the code!

<iframe src="https://cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Ftenor.com%2Fembed%2F5888486&amp;display_name=Tenor&amp;url=https%3A%2F%2Ftenor.com%2Fview%2Fmeditation-hippie-patrick-patrick-star-spongebob-squarepants-gif-5888486&amp;image=https%3A%2F%2Fc.tenor.com%2FJAa6q0pMBQMAAAAC%2Fmeditation-hippie.gif&amp;key=a19fcc184b9711e1b4764040d3dc5c07&amp;type=text%2Fhtml&amp;schema=tenor" width="600" height="400" frameborder="0" scrolling="no"><a href="https://medium.com/media/b667f8fae111d0696714270cb59d5dcc/href">https://medium.com/media/b667f8fae111d0696714270cb59d5dcc/href</a></iframe>

To demonstrate that, I have [**funInJS**](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js)

Talk is still cheap.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869117586/YND89vY1F.png)

1.  An array starting with 0 the index and 0 length
2.  [addElement()](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js#L6) function as .push() increment the length by 1.

So, internally it is treated as an object which is an index as key and value as your "value"

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869119177/wgKjxuQgX.png)

How JavaScript might be treating an object as an array

But for users, it will always be as follows:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869120481/8qZdYgrvH.png)

### Limitations:

As I wrote this, this is still a baby array that is identical to an array but not the whole array, which we use in daily JavaScript. I won’t even recommend this.

Currently, This only supports number and string. It doesn’t support arrays or objects as values yet. Maybe on the next iteration.

Likewise, I have implemented below methods:

1.  [deleteElement()](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js#L11) as in .pop() (need to improve based on location or value) \[Accepting PRs\]
2.  [maximumElement()](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js#L20) Get the maximum element.
3.  [secondMaximumElement()](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js#L34) : Get the 2nd maximum element.
4.  [checkIfArrayIsSorted()](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js#L53) : Check if an array is sorted or not.
5.  [printMeReverse()](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js#L72) : Print the array in reverse order
6.  [searchByIndex()](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js#L84) : Search by index to know the value.
7.  [searchByValue()](https://github.com/TheRakeshPurohit/fun-in-js/blob/main/jan62021.js#L92) : Search by value to know the position.

<iframe src="https://cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Ftenor.com%2Fembed%2F16045826&amp;display_name=Tenor&amp;url=https%3A%2F%2Ftenor.com%2Fview%2Fhot-so-hot-summer-sweating-sweating-hard-gif-16045826&amp;image=https%3A%2F%2Fc.tenor.com%2FjAijH_Fof_YAAAAC%2Fhot-so-hot.gif&amp;key=a19fcc184b9711e1b4764040d3dc5c07&amp;type=text%2Fhtml&amp;schema=tenor" width="600" height="400" frameborder="0" scrolling="no"><a href="https://medium.com/media/39f5efc06aed45bfd4cd284ac2f89c4a/href">https://medium.com/media/39f5efc06aed45bfd4cd284ac2f89c4a/href</a></iframe>

We still have a highway to implement like filter,shift ,unshift, every,some, forEach, map, reduce, fill, etc.

Well !! Numerous senior engineers will peruse this article. Go ahead and remark or give criticism. I would invite your perspectives to connect and develop.

I should go now for another article.

<iframe src="https://cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Ftenor.com%2Fembed%2F17625272&amp;display_name=Tenor&amp;url=https%3A%2F%2Ftenor.com%2Fview%2Fphir-hera-pheri-theek-hai-bhai-mai-chatla-hoon-mai-chalta-hu-thik-hai-bhai-gif-17625272&amp;image=https%3A%2F%2Fc.tenor.com%2F6oMzdz-_96YAAAAC%2Fphir-hera-pheri-theek-hai-bhai.gif&amp;key=a19fcc184b9711e1b4764040d3dc5c07&amp;type=text%2Fhtml&amp;schema=tenor" width="600" height="400" frameborder="0" scrolling="no"><a href="https://medium.com/media/871075fbfcc2cc000aca47ecf2315f32/href">https://medium.com/media/871075fbfcc2cc000aca47ecf2315f32/href</a></iframe>

[LinkedIn](https://www.linkedin.com/in/therakeshpurohit/) [Twitter](https://twitter.com/iRakeshPurohit) [GitHub](https://github.com/TheRakeshPurohit)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869123029/iTBB9K3dy.gif)