# 🎿 Bootilities
A set of utilities generated with Bootstrap 5 to mimic Tailwind CSS functional paradigm

**Disclaimer**

I love [Tailwind CSS](https://tailwindcss.com) as much as the next guy, so much that I decided to use Bootstrap's brand new utility API to port some of that magic over.

**Bear with me...**

I'm just a developer and the majority of my projects require quick iteration and for the most part, I don't have a designer at my disposal.
This means that, even though I like designing webpages, I don't have the time or patience to come up with a robust and consistent design/component system from scratch for every project I work on.

Tailwind CSS is awesome with its utility-first approach, which comes in handy when you need the freedom to work on custom designs.
However, since it's a very thin abstraction layer over pure CSS styles, you are on your own - which is both good and bad depending on what you need.
In my case, I just want to work on some functionality and see things on the screen as soon as possible and Bootstrap has almost anything you might need out-of-the-box.

**About components & Abstractions**

Although you can extract your utilities into components to accommodate your application design requirements with Tailwind, with long-term applications, chances are you will eventually wind up in the same place: with a custom framework that has buttons, cards, tables, dropdowns, and so on, with the exception that **you** are the one that has to keep it consistent. It's a lot of work if you are not up for it.

> The recommended way to work with Tailwind is about abstracting your code into reusable components. But after trying this first I have to admit that for large projects it tends to get very repetitive very fast. That is, unless you already have a established component system at your disposal of course - like Tailwind UI. Having tried that multiple times in different projects in the past, I feel that it's just an extra step that generates unwanted overhead in my projects. Also, consider this: Instead of waiting for patterns to emerge so you can then extract and refactor your code into components, you can start your project with the most common abstractions from the beggining. Besides that, if you don't find what you need or you need a super specific component, you can just go ahead and create it with CSS as you normnally would.

Because of this, I think Bootstrap is an excellent choice if you want a full-fledged framework to help you focus on delivering value as quickly as possible. Besides that, with Bootstrap 5 you have a new utility API at your disposal that will boost your productivity - just no leaving anything behind.

**But TailwindCSS is awesome**

Yes, it is and Bootstrap is as well. It's not a dychotomy, two things **can** be true at once. I believe both tools were created by two of the most capable people I've ever known and are excelent at solving different problems. I've tried both approaches and saw where and when each one of those falls short for my use-case, so here's my attempt to bridge that gap. I don't expect anybody to be convinced only by my words, try it and see for yourself.

**Why didn't you implement Bootstrap in TailwindCSS**

This crossed my mind at one point and I think it could be a valid approach as well. But I was not up for the sheer amount of work that would go on creating and maintaining it. Bootstrap is a very mature and battle tested framework, so the decision on what direction to go was made simpler by that fact. Also, I was catching myself importing Bootstrap components like dropdowns, modal and popovers on my Tailwind projects more frequently that I'd care to admit just for the ease of it, so...

# Installation

```
npm install bootilities --save
```

**⚠️ Note About PurgeCSS**

One of the main disadvantadges of any framework that generates CSS dynamically is that your output files can grow quite large if you don't take proper care. Even though the library is segmented in logical groups that could be imported individually I heavily recommend that you use [PurgeCSS](https://purgecss.com) from the start - even for development. This can greatly reduce the size of the output file and provide a better experience while developing. I'm also looking on providing options and switches to conditionally generate parts of the utilities to better improve the end user experience.    
