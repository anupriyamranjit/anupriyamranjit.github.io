---
layout: post
title:  "Leetcode - Mastering DFS"
date:   2024-05-01 20:12:33 -0400
categories: Interview
tag: [SWE, Interview]
excerpt: "The blog post discusses mastering Depth-First Search (DFS) for coding interviews, aiming to improve speed in writing DFS code. It outlines several questions tackled to understand DFS better "
---

Hi! I'm currently grinding a new grad role and I am going over all the key concepts needed for interviews. 


The first one I wanted to talk about is DFS


Here are the question I did to learn more about it:

I am also trying to improve how fast I can write the DFS code as one of my previous interviews I ran out of time thinking about it

1. [Number of Islands](https://leetcode.com/problems/number-of-islands/){:target="_blank"}
2. [Max Area of Islands](https://leetcode.com/problems/max-area-of-island){:target="_blank"} (Time Taken to Write Code: 6:10)
3. [Pacific Athlantic Flow](https://leetcode.com/problems/pacific-atlantic-water-flow){:target="_blank"} 
4. [Surrounded Regions](https://leetcode.com/problems/surrounded-regions){:target="_blank"} (Time Taken to Write Code: 9:36)

# General Idea and Code Structure

{% highlight python %}

def wrapperclass(self, grid):
  rows, cols = len(grid), len(grid[0])

  visit = set()

  def DFS(row, col):
    if((row,col) in visit):
      return ___

    if(row < 0 or row >= rows):
      return ___

    if(col < 0 or col >= cols):
      return ___
    
    // Other conditions 


    // Add to visited

    visit.add((row, col))

    // Iterate Neighbors



    directions = [(0,1), (0,-1), (1,0), (-1,0)]

    for dr,dc in directions:
      // Deal with neighbors using
      DFS(row + dr, col + dc)

    // Deal use recursive DFS to make DFS_RESULT
    return DFS_RESULT
  
  // Iterate through graph
  for r in range(rows):
    for c in range(cols):
      // Find valid node and run 
        DFS(r,c)
  

  return final_result
  



{% endhighlight %}






