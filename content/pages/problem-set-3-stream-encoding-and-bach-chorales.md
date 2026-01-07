---
content_type: page
description: Description of PSet 3
draft: false
title: 'Week 3: Problem Set 3: Stream Encoding and Bach Chorales'
uid: ebe6f16f-9333-4210-af2a-a8bda2585efc
---
This short problem set will help you solidify your ability to work with Streams: constructing them, iterating over them by hand, and then using recurse() and flatten(). You can also filter them, work with offsets, and work with attributes on their contained notes.

File: {{% resource_link "8b864aaa-0b30-482d-93d4-72bff2defb3e" "Problem Set 3 (IPYNB)" %}}

## Discussion: Shortest Path—DFS or BFS?

A question arose in class about whether we should use depth-first search or breadth-first search to find the shortest path between two points. And I was thinking about the next music theory question so I didn't give a great answer.

I'd lean more towards breadth-first search, the logic being, if you're at point D and want to get to point Z, and from D you can get to A, B, and C, would you prefer to go to A and then all of the places you can get from A before seeing if B or C are actually the same as Z? If you're in Chicago and want to get as quickly as possible to Detroit, would you search first if Amsterdam to Zurich to Mumbai is the fastest route before first seeing if there's a direct flight from Chicago to Detroit?

But I spaced partly because neither BFS nor DFS is the best answer. (Also, unless I'm mistaken, there's no completely solved solution to the problem). What you'd probably want is a heap structure or priority queue (both more similar to BFS than DFS, but not identical), so that you first look at the solution that takes the shortest amount of time, and then put into your heap the next destinations with the shortest time, adding the time it took to get there (and keeping a sort of *visited* set to see what you've already seen). Someone in class mentioned using an A\* (A-star) algorithm, which could also speed up the work.

Because musical notes (and measures, etc.) have both a start and an end time, and we often want to answer questions such as "What chords are playing at the same time as Chord X?" I've spent more of my life learning, implementing, and speeding up a search called "interval tree." Thus, my work on A\* and other shortest path algorithms has taken a back seat to the intricacies of interval trees.

Note: if you ever end up needing max heaps or min-max heaps and find the Python **heapq** library as inscrutable (and non*\-Pythonic* as I have, I made an alternative implementation called "heap-class" {{% resource_link "7721e438-228e-492c-b4a1-9b142b3f3280" "https://pypi.org/project/heap-class/" %}}, which you can use to solve any problems that you think are best solved with heaps.