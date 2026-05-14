---
title: "Is React 18 overhyped?"
seoTitle: "Why React 18"
seoDescription: "There is a buzz around the ReactJS developers around the web and this is because ReactJS v18 is out. Does it worth the attention?"
datePublished: 2022-07-15T18:26:01.000Z
cuid: cl5ng5c5d036vnjnvh8y1cj43
slug: is-react-18-overhyped
canonical: https://therakeshpurohit.medium.com/is-react-18-overhyped-4d305c26441?source=rss-415d4a54ac94------2
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1657869143151/uNbXyAqy4.png
tags: javascript, react, server-side-rendering, react18

---

As a front-end developer, you must have come across articles titled as follows :

1. What’s new in React 18?
    
2. Should you learn React 18?
    
3. React18: Features and updates
    
4. The Complete Guide to React 18
    
5. React 18 will change front-end development.
    
6. Okay, 5th one was made-up…!!
    

All I’m trying to say, blog authors have done their best to draw awareness towards the upcoming release of React 18. My question is, “Does it worth it?”

To answer that, we will see [“What’s new in React 18?”](https://medium.com/@therakeshpurohit/is-react-18-overhyped-4d305c26441) according to the official [plan](https://reactjs.org/blog/2021/06/08/the-plan-for-react-18.html).

1. [**Automatic batching**](https://github.com/reactwg/react-18/discussions/21) **for fewer renders**
    
2. **New API:** [**startTransition**](https://github.com/reactwg/react-18/discussions/41)
    
3. [**New Suspense SSR Architecture**](https://github.com/reactwg/react-18/discussions/37)
    

### 1\. Automatic batching

Till React 17, the only event listeners have the feature of arranging multiple **setState**.

> A piece of code is worth a thousand words.

<iframe src="https://cdn.embedly.com/widgets/media.html?src=https%3A%2F%2Fcarbon.now.sh%2Fembed%3Fbg%3Drgba%252874%252C144%252C226%252C1%2529%26t%3Dmaterial%26wt%3Dnone%26l%3Dauto%26ds%3Dfalse%26dsyoff%3D20px%26dsblur%3D68px%26wc%3Dtrue%26wa%3Dtrue%26pv%3D56px%26ph%3D56px%26ln%3Dfalse%26fl%3D1%26fm%3DFira%2BCode%26fs%3D14px%26lh%3D152%2525%26si%3Dfalse%26es%3D2x%26wm%3Dfalse%26code%3Dfunction%252520handleClick%2528%2529%252520%25257B%25250A%252520%252520%252520%252520setCount%2528c%252520%25253D%25253E%252520c%252520%25252B%2525201%2529%25253B%252520%25252F%25252F%252520Does%252520not%252520re-render%252520yet%25250A%252520%252520%252520%252520setFlag%2528f%252520%25253D%25253E%252520%2521f%2529%25253B%252520%25252F%25252F%252520Does%252520not%252520re-render%252520yet%25250A%252520%252520%252520%252520%25252F%25252F%252520React%252520will%252520only%252520re-render%252520once%252520at%252520the%252520end%252520%2528that%2527s%252520batching%2521%2529%25250A%252520%252520%25257D&display_name=Carbon&url=https%3A%2F%2Fcarbon.now.sh%2F%3Fbg%3Drgba%25252874%25252C144%25252C226%25252C1%252529%26t%3Dmaterial%26wt%3Dnone%26l%3Dauto%26ds%3Dfalse%26dsyoff%3D20px%26dsblur%3D68px%26wc%3Dtrue%26wa%3Dtrue%26pv%3D56px%26ph%3D56px%26ln%3Dfalse%26fl%3D1%26fm%3DFira%2BCode%26fs%3D14px%26lh%3D152%252525%26si%3Dfalse%26es%3D2x%26wm%3Dfalse%26code%3Dfunction%25252520handleClick%252528%252529%25252520%2525257B%2525250A%25252520%25252520%25252520%25252520setCount%252528c%25252520%2525253D%2525253E%25252520c%25252520%2525252B%252525201%252529%2525253B%25252520%2525252F%2525252F%25252520Does%25252520not%25252520re-render%25252520yet%2525250A%25252520%25252520%25252520%25252520setFlag%252528f%25252520%2525253D%2525253E%25252520%252521f%252529%2525253B%25252520%2525252F%2525252F%25252520Does%25252520not%25252520re-render%25252520yet%2525250A%25252520%25252520%25252520%25252520%2525252F%2525252F%25252520React%25252520will%25252520only%25252520re-render%25252520once%25252520at%25252520the%25252520end%25252520%252528that%252527s%25252520batching%252521%252529%2525250A%25252520%25252520%2525257D&image=https%3A%2F%2Fcarbon.now.sh%2Fstatic%2Fbrand%2Fbanner.png&key=a19fcc184b9711e1b4764040d3dc5c07&type=text%2Fhtml&scroll=auto&schema=carbon" width="1024" height="480"><a href="https://medium.com/media/c64f4809cc3eb301225bf16ab0ce26dc/href">https://medium.com/media/c64f4809cc3eb301225bf16ab0ce26dc/href</a></iframe>

From React 18 it will support [inside of timeouts, promises, native event handlers or any other event will batch the same way as updates inside of React events.](https://github.com/reactwg/react-18/discussions/21#:~:text=inside%20of%20timeouts%2C%20promises%2C%20native%20event%20handlers%20or%20any%20other%20event%20will%20batch%20the%20same%20way%20as%20updates%20inside%20of%20React%20events.)

#### What if I don’t want this feature?

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869128770/OL0sdvTds.png align="left")

### 2\. startTransition

Suppose,

1. You’ve got an input element that causes an \`onChange\` event
    
2. The value gets updated.
    
3. On value change, you fire a query for data
    
4. Render the result on the screen.
    

It looks shallow but if we see rendering cycle and performance it may cause issues on slow environments depending on the computations going on such as animations and transitions and more interactive UI transactions.

In this case, some of us might have used **throttling** or **debouncing** or **setTimeout** but that doesn't stop the query from performing heavy UI renders.

#### This is the React 18 way!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869131075/07zP5Q5_e.png align="left")

Anything written inside **startTransition** will be chronicled as “non-urgent” by React. So if the user keeps changing the input value it will pick only the latest value and fire the query to get data! ( blushing while writing this line)

Quote this.

> [Transitions lets you keep most interactions snappy even if they lead to significant UI changes. They also let you avoid wasting time rendering content that’s no longer relevant.](https://github.com/reactwg/react-18/discussions/41#:~:text=Transitions%20lets%20you%20keep%20most%20interactions%20snappy%20even%20if%20they%20lead%20to%20significant%20UI%20changes.%20They%20also%20let%20you%20avoid%20wasting%20time%20rendering%20content%20that%27s%20no%20longer%20relevant.)

**startTransition** doesn’t schedule the execution for later like setTimeout, rather it invokes immediately and synchronously.

Moreover, setTimeout doesn’t allow user interruption while startTransition allows the interruptions with the latest value only.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869136727/k6ZS4U1MW.jpeg align="left")

Photo by [Mike van den Bos](https://unsplash.com/@mike_van_den_bos?utm_source=medium&utm_medium=referral) on [Unsplash](https://unsplash.com?utm_source=medium&utm_medium=referral)

**Loading….**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869138443/8s3fO6hf0.png align="left")

This is how you can optimize the user experience. Users will get a spinner only while data is being prepared. No need to write brittle asynchronous code.

### 3\. Suspense SSR Architecture

Don’t misunderstand it with the [server component](https://reactjs.org/blog/2020/12/21/data-fetching-with-react-server-components.html) which is a completely different thing.

Server-Side-Rendering provides optimized hydration which leads to better SEO and indexing as well as user engagement, [FMP](https://web.dev/first-meaningful-paint/) and [FCP](https://web.dev/first-contentful-paint/).

SSR renders all HTML first and serves to the user so users can get the content, then loads JS file for interactive UI like button clicks, transitions, animation etc.

There are two new things:

1. *Streaming HTML*
    
2. *Hydration.*
    

Currently, it's “all or thing” there is no opt-in. In React 18 you can specifically choose which to stream first/last and which component to hydrate first/last. Totally up to you. Great, right?

### **Bonus**

**\=&gt; useId :**

To give a unique id, we rely on packages like [UUID](https://www.npmjs.com/package/uuid) (not to mention why). React has its API for that, which is globally unique. See code below.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869140368/HSjU0xg5R.png align="left")

No need to call the function N time to get N new ids.

**My opinion:**

1. Automatic batching =&gt; Pass
    
2. startTransition =&gt; Pass
    
3. SSR =&gt; Pass
    

Yet, I believe that React 18 doesn’t merit the current hype. Not everyone running projects on React 17 are going to run `ncu -u` and update the react and react-dom packages.

Let me know your feedback !!

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1657869141983/-f2lPBfgb.gif align="left")