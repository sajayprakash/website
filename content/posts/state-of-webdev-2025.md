---
title: "The current state of Web Development: A noobs perspective"
date: 2025-01-10T12:32:42+05:30
description: I have been learning and doing web development for the past 3 years starting with HTML, CSS and moving over to React and React frameworks. This post goes over why I think the web development ecosystem needs a change and is not beginner friendly.
tags: ["web-dev", "programming", "career"]
# summary: ""
# featureimage: ""
# featureimagecaption: ""
# showDateUpdated: true
# showTableOfContents: false
# showComments: false
# showAuthor: false
# authors: []
# sharingLinks: false
draft: falses
---
## My background

When I finished school and joined my college, I had a decent understanding of Python, C, Java and also have done some basic HTML/CSS in my junior school days. I have always been interested in building my own applications from the design to front-end and back-end. This was when I decided I will focus on learning Full Stack Development and so I began searching reddit threads and other websites such as [GeeksforGeeks](https://www.geeksforgeeks.org/) for resources and to understand what would be the ideal roadmap to follow. Since everyone recommended starting with vanilla HTML/CSS and JavaScript, I began to learn them and also built a couple of your typical recipe websites, nothing too crazy. Then, I wanted to start building applications and connecting my application with a backend, so like before I searched the Internet to check where to start and this was the second time in my life I was overwhelmed by the number of pathways and options I had. The first time and last time I felt this way was when I began my Linux journey at the age of 14 where I had to choose between at least 10 Linux distributions. Don't get me wrong, having the freedom to choose is great and promotes healthy competition but as a beginner who knows nothing it is very overwhelming and creates a sense of anxiety if we will make the wrong choice. Since I had no clue what to pick between React, Angular, Vue, Svelte for front-end, Bootstrap, Tailwind, vanilla CSS or some UI library for the styling, MongoDB, PostgreSQL, MySQL, SQLite for the backend, JavaScript or TypeScript for the programming language (TypeScript is just JavaScript with types but as a noob I had no idea what that was) I just chose the popular ones.

Here was my final choice:

- React
- JavaScript/TypeScript
- Tailwind CSS
- PostgreSQL/MySQL
## Tutorial Hell
After making my tech stack choice, I began searching the internet for tutorials and I was surely not disappointed - There were hundreds of tutorials on "how to build XYZ" and like most people I began following the tutorial, line by line. In the beginning, I was pretty proud of myself when I built my first fully working React website but as time went by I was not able to understand the code which I wrote tirelessly by copying the 4 hour long videos, this was when I kept switching tutorial after tutorial searching for the "right" tutorial that will teach me everything. This led me down the rabbit hole of tutorial hell.[^1]

[^1]: Tutorial hell is where you write code that others are explaining to you how to write, but you don’t understand how to write it yourself when given a blank slate [boot.dev](https://blog.boot.dev/education/building-your-first-coding-project/#).

{{< youtubeLite id="O99NMMk4I4g" label="Escaping Tutorial Hell" >}}

Then I came across this video by [LowLevelLearning](https://www.youtube.com/@LowLevelTV) which kinda helped me move away from tutorial hell, so I picked a simple project and built it. Which was when I built this [Japanese Flashcard Site](https://japanese-flashcard-site.vercel.app/) which I was pretty proud of, I learnt how to do component based development, use React hooks such as `useState` and `useEffect` and also setup Tailwind CSS. 

## Transition to Next.js
So far I had been creating single-page applications and I wanted to create an application with multiple routes. This is where I came across my first hurdle where I learnt that React does not support multiple routes by default, instead I have to use a router such as [React Router](https://reactrouter.com/).  It was not that complicated to setup but I found it weird, why would anyone want a framework that only supports single-page applications? - and the solution to this recommended by most people was to use [Next.js](https://nextjs.org/) which is a React framework (A framework of a framework lol). Next.js had support for multiple routes and came with a neat CLI that setup Tailwind CSS by default. To this day, Next.js is the primary framework I used to develop full stack applications but this too had it's downsides. A common complaint of Next.js was that it was controlled by [Vercel](https://vercel.com/) which also meant that it could lead to a vendor lock-in[^2].

[^2]: vendor lock-in is also known as proprietary lock-in or customer lock-in, makes a customer dependent on a vendor for products, unable to use another vendor without substantial switching costs [Wikipedia](https://en.wikipedia.org/wiki/Vendor_lock-in).

{{< youtubeLite id="Jw8sXzaZUDQ" label="Breaking Up with Next.js" >}}

This video goes over some of the similar opinions I had about Next.js, it really felt like Next.js was becoming a product of Vercel that ties deeply with its platform and services and they caused me major issues when they chose to use React 19 in Next.js 15 when it was still a release candidate which caused peer dependency issues and it still baffles me how they chose a non-stable version of React in their major release. It also felt like Next.js was too opinionated which forced me to develop my apps a certain way with a specific structure. 

Ignoring these issues, I developed my applications in Next.js and overall had a pretty decent experience with the occasional hiccups such as Hydration errors, server components, client components, slow rendering and page refresh, etc. This was the beginning of my frustration with the JavaScript ecosystem.

## JavaScript is a terrible language
The more I used JavaScript/TypeScript, the more I hated it. It just felt wrong using it to create my applications and websites. There are soo many weird issues within the language itself, don't believe me? Take a look at this repo

{{< github repo="denysdovhan/wtfjs" >}}

It contains a set of examples that represent how poorly designed the language itself is. This isn't some weird set of edge cases that don't affect the daily code, it genuinely caused some weird bugs and errors that were messing with your brain. 

It also felt pretty bloated and Node.js eats up so much of your memory and has memory leaks sometimes which lead to memory usage spikes. JavaScript was such as problem that Microsoft decided to create TypeScript which introduced types. TypeScript fixes some of the issues that vanilla JavaScript has and honestly I don't know why anyone would not use TypeScript as it provides a better developer experience but still the more I kept coding the more I hated the web development ecosystem.

## Moving away from Web Development
I am extremely disappointed with the current state of web development and slowly trying to transition away from it as I don't think it is for me. I will do an update on this post if I fully commit myself to another field and as for now I'm going to continue doing web dev despite not liking it. I feel the market is over-saturated with web developers and people who have learnt a specific tech stack such as MERN[^3].

[^3]: MERN is a pre-built technology stack based on JavaScript technologies. MERN stands for MongoDB, Express, React, and Node, after the four key technologies that make up the stack [MongoDB](https://www.mongodb.com/resources/languages/mern-stack).

This also makes getting a job pretty challenging as there are too many people applying for the same job and the competition is really high. This is not a bad thing, it is good and says that the field is still in demand but it's also really frustrating for someone who is new to this field.

As a first step to moving away from web development and JavaScript frameworks, I decided to recreate my website which was previously using [Astro](https://astro.build/) to [Hugo](https://gohugo.io/). It's a little funny how my [original site](https://github.com/sajayprakash/old-personal-site/tree/hugo-site) which I made during my high school was also made using Hugo and I have gone around a full circle to come back to using it.

## Skill Issue?
This post was not really made to discourage anyone who is interested in web development. Maybe all of this was just a skill issue[^4] and I approached this in the wrong way. If you have any opinions or suggestions feel free to comment below or message me via my socials and if you are starting out then I highly recommend you to try all of this out yourself and form your own opinion, at the end of the day this is mine.

[^4]: a snide remark used to suggest that the root cause of a problem lies with the incompetence/lack of skill of the person expressing said problem [Urban Dictionary](https://www.urbandictionary.com/define.php?term=skill%20issue).
