# lewissaunders.github.io

#### Technical Report
This assessment required us to create a portfolio page using jekyll and github pages, it required a minimum of three pages, a navigation bar and icon, at the top of every page. We also were required to show the wireframes for each page. (shown below)
The idea behind this assessment was that it would give us something to work off, if we chose to, as a portfolio that could be given as a card with a website URL.

##### Process

Initially, I wanted to start by creating a github pages repo, and working from there, however, at that point I wasn't able to get my head around how to set it up correctly. Mainly because I kept running into issues regarding having jekyll bundles set up on the required repo.

So instead of getting fed up and stuck I decided to create a local repository and work on the jekyll site itself. While working on the website, there were many issues that I ran into.

The first issue I ran into was the need for the index.md page; in general, I like to be able to have my files named in an organized format where the word before the document type is respective of what it is. This meant that if i wanted to use the skills page as the home page, i had to accept that it would be under the title of index.md. (when the name was changed from index.md to something like skills.md, it broke the landing page layout/design).

Following this, it came to my attention that it was necessary for index.md to be the landing page, because no matter how many different yml front matter changes or replacements i made, it would not accept anything else to be the landing page.
This was also the other factor which caused me to set up index.md as my skills page.
 
Another issue I ran into was the line "Click here to Subscribe to RSS" or something similar. It was part of the base template (Minima), and I couldn't stand it being there. However, when i tried to remove it through the base HTML files, it would reappear whenever the server was restarted. (This happened with any HTML changes done through the Site Folder). The work around for this was to copy the template from the actual GEM folder into this repository which allowed me to edit it freely (as well as the CSS). I believe this occurred do it the copied template having a further up in the hierarchy.

Had to gain a better understanding of CSS (specifically grids etc.)
I'll be frank, my applicable HTML and CSS skills aren't where I want them to be, so I had to do a lot fo playing around to get the grid sorted and appearing the way i wanted it. The Site i was using to help me was using a line called grid-gap, which I later found was no longer usable. However, i did find out that instead we just use `grid-template-rows` and `grid-template-columns` instead.

Following these hiccups, I managed to get a result that i was happy with. The site has three pages, of which, the skills page is the home/landing page, as well as having a navigation bar on the header of each page, as well as an icon (my face).

##### Progress

Regarding progress of this website, I would say it is at 50% of it total potential. There is a lot room for improvement, especially in regards to the projects. The empty white space on some of the pages could be filled with something (potentially an image) and the overall icon shape doesn't sit well with me. However, these are all things that can be added in the future. The time it took to get where i have, is by no means acceptable, however, I know that with repetition, my skills will grow exponentially and allow me to gain the confidence in myself. If I were to continue to develop this page after the assignment is handed in, I would make it so the grid of projects will each link to their own separate page, giving more detail as to what was involved in each. I would also like to spruce up the css quite a bit, and make it more "my own" through different shapes, and color schemes.

##### Results
Overall i feel that while this isn't my best work by far, it's something, and it has the potential to be something even greater if i continue to work on it.
Below i will give a more broken down explanation of what the different files are, and what they achieve:

We have the main three .md files (Articles/index/projects), these three are the documents that turn into the different pages of the website, we do however, also, have another .md file in the _posts folder. The reason for their separation is because while the post .md file is also a page, the title, (YYYY-MM-DD-"") tell jekyll that it belongs on the Articles page, as a clickable link to said page.
Following that we have the _config.yml file, which when data is added correctly, automatically updates the HTML accordingly, for example, changing the "title:" in the .yml file will change it from Portfolio, to what ever is chosen, and will be updated on every page.
The _layouts folder contains the HTML of the 4 different types of page layouts that can be given through the front matter in each .md file. I mentioned earlier that i had to bring in a secondary template folder, as I wasn't able to edit the initial without it automatically reverting changes i made once i reset the server. This was the workaround.
In the _includes folder is the Header, Footer, Head, and other HTML files that make up different parts of the page. I was required to play around with the Header.HTML in order to get the icon configured into the correct location.
The _sass folder contains all the applicable CSS to this website, i specifically had to play around with the _layouts.scss file in order to get the grid working on the projects page.

#### Wireframes

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
The projects page will have a grid layout initially showing up to 8 icons with the names of the projects in boxs. If the user wishes to find out more about said project, the will be able to click on it, and follow through to a new page. (new pages will not be available until projects have been done).

#### Journal Reflections

##### Lab 3 Reflection
##### Lab 4 Reflection
##### Lab 5 Reflection