---
layout: post
title:  "How does React work"
date:   2024-05-01 20:12:33 -0400
categories: React
tag: [SWE, Frontend]
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

#### HTML Rendering

This HTML that is sent to you is then converted into a tree structure made up of Nodes let's show an example


```html
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
  ```


  Made into 
![Alt text for broken image link](/assets/html_dom.png)





