---
layout: post
title: "Jekyll and Website Creation"
date: 2022-11-28
category: projects
---

The creation of a website is to many their first exposure to programming. The meticulous process of learning HTML followed by an introduction to CSS is found within many elementary programming courses. Despite this I have never really set out to create more than a basic website. Therefore, in an effort to learn basic web fundamentals - which will invariably become useful - I have decided to create a basic blogging site with the Jekyll framework.

### Jekyll
*Jekyll* is a static website generator, with it being the most popular one. A static website generator functions by using a series of templates and text files as to create a website. This allows for easy expansion of new pages without the need to spend time programming a website for every page. *Jekyll* runs on *Ruby*, a language known for its web integration and ability to interface with server-side applications.

For this project *Jekyll* was chosen as it minimizes the programming required for future blog posts, a massive benefit for blog posts as it allows for more focus on research. This is coupled with its extensive documentation which allows for easy troubleshooting. The *Liquid* scripting language found within the `.html` also proves helpful if not a little too simple.

The creation of a Jekyll project is fairly simple, with the command `jekyll new <project-name>` creating a new project with the base theme *Minima*. While the Minima theme leaves a lot to be desired it does function as a nice base to build off. This is due to it having a nice system of generating posts, as well as the skeleton structure of a website. It is off this that the website will be built.

### HTML
HTML functions as the basic tool to create the overall structure of the website though the Jekyll templates. The main `_layouts` found within the website are the `default` and `home` pages. The default page follows the basic structure outlined by *Minima*. It is used to pull together the core elements of the website. This is used all throughout the website as the basic for all other layouts. Beyond these templates there are also `_includes` which are items which modify the look of the site. These are called by the layouts and include the sidebar, footer and other features. 

#### Sidebar
A large part of the website was the creation of a prominent sidebar used for navigation. This sidebar lists the website's title, a quote and a list of possible directories. These directories are the *Home*, *About*, and a dynamically generated list of categories. This was done through the use of liquid as to create list items based on the categories specified within the markdown file categories.

Adding a bold style to the selected subcategory of page is another addition to the sidebar. This was done once again with liquid which allows for tests of logical statements. With cases where the link contains the name of a subcategory adding a bold styling to the sidebar.

### Styling
A large part of creating a website is dealing with the design of the site, which is done through CSS. For this website all the styling sheets were done with *Syntactically Awesome Style Sheets*, a CSS superset which seems to be the standard for Jekyll websites. If I was better orientated with CSS this tool would prove to be even more useful however for this blog I just used the basic tools provided by CSS and the theme.

#### Fonts
Fonts set the tone of the site and as a result I have decided to pick a non-standard font. To his end instead of the web standard of *Helvetica* I chose to use *IBM Plex*, and *Fira Code* for code snippets. *IBM Plex* is a fairly basic font which looks similar to *Helvetica* with more of a focus squared off letters. This is coupled with the fact it is made by IBM which has a nice relation to the history of computers. *Fira Code* is a font based off of Fira by Firefox. It has programming ligatures which I believe look nice.

#### Phone Support
One of the difficulties with a sidebar is that is proves difficult to use on phones or devices with a smaller aspect ratio. To mitigate this styling was used as to set the navigation bar to the top of the screen. Removing elements such as the quote as to provide a basic element for site navigation. Removing its fixed position allows for the article to be easier read. While the code to do this wasn't the best, as I am almost sure there is a better solution, it proved to fulfill the basic needs of phone support.

### GitHub Pages
The last process in the creation of a website is finding a way to host it. For this site I decided to use GitHub Pages as it allows for free hosting with strong integration with Jekyll. This selling point, coupled with version control features provided by git make it an attractive option for anyone who needs to host a website with low overhead. 

### Conclusion
Overall from this the following site that you are reading from was created. Through this whole process I have personally learnt the more basic elements and design techniques used within web development. I hope that in the future I can use similar static site generators in the quick deployment of applications.

### References
- Jekyll Documentation: https://jekyllrb.com/
- Liquid Documentation: https://shopify.github.io/liquid/
- Basis for Sidebar Look: https://hyde.getpoole.com/