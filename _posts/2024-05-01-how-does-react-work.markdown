---
layout: post
title:  "How does React work"
date:   2024-05-01 20:12:33 -0400
categories: React
tag: [SWE, Frontend]
excerpt: "The article provides a succinct introduction to React's function in rendering HTML for web apps. It mentions prominent companies that use React and simplifies the process of web content delivery. The main focus is on explaining how React renders HTML, showcasing the conversion of HTML into a tree structure of nodes using an example snippet and an accompanying image. Overall, it aims to give readers a basic grasp of React's role in rendering web content."
---
This article is a quick overview of React and how it renders HTML that you see every day

## Who uses React
React is used by multiple large companies 
- Facebook (Meta)
- Netflix
- Dropbox
- Airbnb

## How does the web show you content?
Through some web magic you get the files from a server ( I don't want to go into DNS and other netwroking concepts in this article)

Now is the real content

### HTML Rendering

This HTML that is sent to you is then converted into a tree structure made up of Nodes let's show an example

#### DOM
{% highlight html %}
  <div>
    <h1>Welcome to My Website</h1>
    <p>Hello, this is a random paragraph.</p>
    <ul>
        <li>Random list item 1</li>
        <li>Random list item 2</li>
        <li>Random list item 3</li>
    </ul>
    <div>
        <h2>Random Subsection</h2>
        <p>More random text here.</p>
    </div>
  </div>
{% endhighlight %}


  Made into 
![Alt text for broken image link](/assets/html_dom.png)

#### CSSOM
A similar procress is also done to the CSS which creates CSSOM that looks like the following

![Alt text for broken image link](/assets/cssom.png)


#### Render Tree
These 2 get combined into somethign called a render tree which only renders the **visible node** (so nodes with display:none are ignored)


![Alt text for broken image link](/assets/rendertree.png)


#### Layout
This render tree is then passed into the layout stage where the size of each element is calcualted 


#### Painting
Finally, after the layout stage we render each element in the correct position



### How are HTML pages updates made?

This may not seem relevant but is important to undertand on why React was created


When changes are made to the HTML the entire DOM is recreated which then recreates the render tree. So this means this is a complete rewrite. This as you can tell can be pretty slow as the render tree needs to remade.


### How is React Different?













