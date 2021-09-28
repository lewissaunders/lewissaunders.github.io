# lewissaunders.github.io

### **Technical Report**
This assessment required us to create a portfolio page using jekyll and github pages, it required a minimum of three pages, a navigation bar and icon, at the top of every page. We also were required to show the wireframes for each page. (shown below)
The idea behind this assessment was that it would give us something to work off, if we chose to, as a portfolio that could be given as a card with a website URL.

#### **Process**

Initially, I wanted to start by creating a github pages repo, and working from there, however, at that point I wasn't able to get my head around how to set it up correctly. Mainly because I kept running into issues regarding having jekyll bundles set up on the required repo.

So instead of getting fed up and stuck I decided to create a local repository and work on the jekyll site itself. While working on the website, there were many issues that I ran into.

The first issue I ran into was the need for the index.md page; in general, I like to be able to have my files named in an organized format where the word before the document type is respective of what it is. This meant that if i wanted to use the skills page as the home page, i had to accept that it would be under the title of index.md. (when the name was changed from index.md to something like skills.md, it broke the landing page layout/design).

Following this, it came to my attention that it was necessary for index.md to be the landing page, because no matter how many different yml front matter changes or replacements i made, it would not accept anything else to be the landing page.
This was also the other factor which caused me to set up index.md as my skills page.
 
Another issue I ran into was the line "Click here to Subscribe to RSS" or something similar. It was part of the base template (Minima), and I couldn't stand it being there. However, when i tried to remove it through the base HTML files, it would reappear whenever the server was restarted. (This happened with any HTML changes done through the Site Folder). The work around for this was to copy the template from the actual GEM folder into this repository which allowed me to edit it freely (as well as the CSS). I believe this occurred do it the copied template having a further up in the hierarchy.

Had to gain a better understanding of CSS (specifically grids etc.)
I'll be frank, my applicable HTML and CSS skills aren't where I want them to be, so I had to do a lot fo playing around to get the grid sorted and appearing the way i wanted it. The Site i was using to help me was using a line called grid-gap, which I later found was no longer usable. However, i did find out that instead we just use `grid-template-rows` and `grid-template-columns` instead.

Following these hiccups, I managed to get a result that i was happy with. The site has three pages, of which, the skills page is the home/landing page, as well as having a navigation bar on the header of each page, as well as an icon (my face).

#### **Progress**

Regarding progress of this website, I would say it is at 50% of it total potential. There is a lot room for improvement, especially in regards to the projects. The empty white space on some of the pages could be filled with something (potentially an image) and the overall icon shape doesn't sit well with me. However, these are all things that can be added in the future. The time it took to get where i have, is by no means acceptable, however, I know that with repetition, my skills will grow exponentially and allow me to gain the confidence in myself. If I were to continue to develop this page after the assignment is handed in, I would make it so the grid of projects will each link to their own separate page, giving more detail as to what was involved in each. I would also like to spruce up the css quite a bit, and make it more "my own" through different shapes, and color schemes.

#### **Results**
Overall i feel that while this isn't my best work by far, it's something, and it has the potential to be something even greater if i continue to work on it.
Below i will give a more broken down explanation of what the different files are, and what they achieve:

We have the main three .md files (Articles/index/projects), these three are the documents that turn into the different pages of the website, we do however, also, have another .md file in the _posts folder. The reason for their separation is because while the post .md file is also a page, the title, (YYYY-MM-DD-"") tell jekyll that it belongs on the Articles page, as a clickable link to said page.
Following that we have the _config.yml file, which when data is added correctly, automatically updates the HTML accordingly, for example, changing the "title:" in the .yml file will change it from Portfolio, to what ever is chosen, and will be updated on every page.
The _layouts folder contains the HTML of the 4 different types of page layouts that can be given through the front matter in each .md file. I mentioned earlier that i had to bring in a secondary template folder, as I wasn't able to edit the initial without it automatically reverting changes i made once i reset the server. This was the workaround.
In the _includes folder is the Header, Footer, Head, and other HTML files that make up different parts of the page. I was required to play around with the Header.HTML in order to get the icon configured into the correct location.
The _sass folder contains all the applicable CSS to this website, i specifically had to play around with the _layouts.scss file in order to get the grid working on the projects page.

### **Wireframes**

![SkillsPageWireframe](/images/SkillsWireframe.PNG "Skills Page Wireframe")
<br>
The above image is a wireframe of what I would like for the Skills page (also will be the landing/home page). The layout of each page will be identical in regards to the footer and the header, however the content on each page will be different. On the skills page, I will most likely have a list of skills. If I wanted to expand on this, each skill could have a paragraph explaining why I possess this skill etc.
<br>

![ArticlesPageWireframe](/images/ArticlesWireframe.PNG "Articles Page Wireframe")
<br>
The articles page wireframe shows that the layout is the same, however each article/blog will be above/below another one. with the most recent appearing at the top. 
<br>

![ProjectsPageWireframe](/images/ProjectsWireframe.PNG "Projects Page Wireframe")
<br>
The projects page will have a grid layout initially showing up to 8 icons with the names of the projects in boxes. If the user wishes to find out more about said project, the will be able to click on it, and follow through to a new page. (new pages will not be available until projects have been done).

### **Journal Reflections**

#### Lab 3 Reflection

##### Pros and Cons of using P5.js library

The topic of P5.js was covered in class as well as through this lab, in the classes we went over how you were able to create 3D images or designs through just JavaScript. In the Lab, we created a table talking about the Pro's and cons of using P5.js. What i've learnt about P5.js is pretty simple, it essentially allows you to be less skilled in HTML and CSS while still allowing you to have the capability to create things that would usually be dependant on it. I like to think of P5.js as a skill tree in an MMORPG (Massive Multiplayer Online Role Playing Game(think World of Warcraft)), that when you specialize into it, it can make having a lower skill level in HTML and CSS significantly less straining.

The biggest thing that i now know compared to before is that P5.js exists, while i don't feel confident in using it, it is something that does interest me, as i find it intriguing that you can use simply JavaScript to create some amazing images/designs. 

The fact that there is something out there that can essentially take the roles of HTML CSS and JavaScript and turn it all into one thing gives me a new understanding of how amazing libraries are, there is so much content that could be created, and shared with others.

Im not entirely sure as to why we have learnt this, but i know that we wouldn't be taught it unless it was something that would be beneficial to us at some point. Even if it isn't, it gives us the opportunity to carry on and learn more about it if it's something that interests us.

I would say that the real life application is dependant on whether or not you get the opportunity to use it in the role you take after study. Even then, from the reviews I have read about it, it's base skill requirement is very low, but its skill ceiling is also high, which usually isn't the case. Essentially it truly is dependant one what the task at hand is, and what are the requirements/barriers to using it.

The way i learnt about P5.js was through Ali's classes, where we created 3D models that were capable of moving in a browser. Outside of class, i did a decent amount of reading about its difficulty (or lack there of) through review sites, or if there was a forum where someone was asking for help, there seemed to be a lot of people willing to help due to it being a product of a previous software/library.

Having the lab will help serve as a reminder of what it can do, and what is needed to perform correctly, if i wish to continue learning, it will most likely be through the several forums available, and through YouTube videos. 

As mentioned above, if i do choose to nourish my craving for knowledge, it will be most likely be done through the media of video. The reasoning behind this is that there is likely to be many different teaching styles available, which can help me in the long run. The reason behind liking videos is that i can take it at my own pace, and pause it, rewind and go over it again if i miss something.

#### Lab 4 Reflection

##### DOM Tree Nodes

Throughout this lab I learnt a lot of different things about the structure of an HTML document, specifically a DOM tree. The repetition of writing out the different elements and Attributes solidified my knowledge of those that i had to type in, for example, I will never forget div, meta, body, label, etc. This lab also allowed me to improve my capability of reading a page of html, and have a better understanding of what i was reading without needing to break everything down. We also went over the different approaches or methods for selecting any element in the HTML DOM Node tree, we listed 3 different approaches, each of which, targeting a different node

Before the lab, my understanding of DOM Node trees was terrible, and it was only by working through it that I understood it. It felt like i was slamming my head against a wall to begin with, but slowly, i started to make progress and was able to figure out how it all fit together. I remember Ali going over the approaches to selecting elements in class (during lockdown), and even that didn't make much sense, but only when i could see the physical layout of the DOM did i start to piece it all together. 

My understanding of DOM trees has gone through the roof compared to when i started the topic, there is always room for improvement however, but if you asked to me make another DOM tree again, i feel that i would be able to do it in under 1/10th of the time it took me. The understanding of the different approaches however is still something that im not 100% confident with, more specifically when or where to apply them, I do believe however that this is something that will most likely be used in the 3rd assignment for this class (WEB503).

As mentioned before i believe that we have been taught the approaches as it will be applicable to the 3rd assignment most likely, and also for any further study we do relating to web design, the DOM tree however i feel is more a tool to help us view the HTML in different ways. This is especially helpful for those that need to see things in multiple ways to understand (Myself).

The real life applications are odd, for example, i can now inspect most web pages and have a read of the HTML and mentally create a DOM tree, which allows me to understand what im seeing quicker, and allows to me to think of how i could change it. The real life applications of the approaches however is most likely going to be for whenever you want to integrate HTML and JavaScript. 

The learning of this topic wasn't easy, and it felt monotonous, up into i made a break through in regards to the mental block, but it really is just a matter of sticking with it until something clicks. I did take many breaks in between attempts as well, so that i was coming back to it with a fresh mindset. I tried to use Youtube videos to also try to explain it in a way that hadn't been already. I know that with the way i like to learn it can be very hard to get a point through, until it does, and most of the time its just a repetition issue. However when it does, im usually capable of replicating the skill necessary.

In order to remember what i learnt, i am able to look over different HTML pages on the web through the inspect tool, which i can then look and see how they've done things, which in turns gives me ideas for future projects etc. Regarding the different approaches to targeting a specific DOM tree node, i do have the journal i wrote for the lab which does have a couple of different examples. From there i will most likely be able to pick up on what ive forgotten, as well as have an understanding of what to look up if i get confused.

Repetition is the key to success with me, and being able to see the results of what i type. in saying that, i think that my knowledge of how to write up, and produce a DOM Tree is pretty good, and won't need much more filling in regards to gaps (that i know of). The approaches however, will come with practice and use in different situations. Which i feel hasn't had a lot of practical uses as of yet.

#### Lab 5 Reflection

##### MVC vs DOM

Throughout this lab there was a lot of information that i had to figure out, whether that be finding the answers online, or asking questions that would get an answer that i understood, and that Ali was able to understand what I was struggling to communicate. The lab was about the difference between an MVC (Model, View, Controller) and DOM (Document Object Model). Essentially the answer came down to the fact that DOM is MVC minus the Model aspect, and a little of the Controller aspect. Whilst a bit more detailed than that, DOM and the View aspect of the MVC are both used to change something that is visible on the webpage. The reason why controller "technically" could fit in there is because it is what's used to manipulate the data. In this lab we also covered 5 different DOM methods, such as selecting an Element based on the id attribute etc.

We had previous discussed DOM Tree Nodes in Lab before this, which allowed us to have an understanding of how those worked. MVC however, was completely new and foreign. After some research and questions, it became apparent that while they both are separate, they do hold similarities. From this lab i gained a new understanding of how two things which are different looking from the outside, can be very similar when you explore what they each actually do. I believe we learnt this because they are both tools that can be used to changed things on a webpage, and we are in fact in the WEB503 class.

The real life applications for this specifically i cannot think of, off the top of my head, but the thought process behind setting two things up next to one another and comparing the differences and similarities will no doubt be a skill that will be beneficial in any scenario of work.

As mentioned above, I struggled to get my head around this until i was able to communicate what part was giving me trouble to understand. I have to thank Ali for being able to give an answer in a way that i was able to understand (no fault on his end, I just struggle with processing certain things). Essentially hammering in that what i was thinking at the time (these two things are very similar) and getting that confirmation gave me the patience to carry on and keep learning about it.

Like all the previous journals, i will be able to refer to my labs as an initial source of information, and from there I will be able to figure out what i want to know, or what im lacking knowledge in. After which, using the resources around me such as YouTube or forums to help.

##### Conclusion

With this reflection I have discovered that the knowledge i had at the start of this course pales in comparison to what i know now, and that whilst i give myself a hard time, its usually only one or two steps that are giving me grief, and once i get past those barriers, its smooth sailing. I know that the knowledge i have gained is impacting the way i approach things and also the consistent issues im encountering are only going to make me better.
