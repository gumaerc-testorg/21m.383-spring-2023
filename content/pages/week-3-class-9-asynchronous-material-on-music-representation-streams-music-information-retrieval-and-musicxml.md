---
content_type: page
description: Videos, readings, and other materials on Music Representation, Streams,
  Music Information Retrieval, and MusicXML.
draft: false
title: 'Week 3: Class 9: Asynchronous Material'
uid: b56750b6-f922-4638-92fd-685623390e9e
---
The next topic moves into a particular representation of CWMN for the computer, the music21 Stream object which can hold notes and much more. Before we begin working with Streams, let us familiarize ourselves with a particular piece of music that we will be working with in this class: J.S. Bach's chorale "Alleluia, des soll'n wir alle froh sein" from Cantata no. 66 *Erfreut euch, ihr Herzen,* designated BWV 66.6.

BWV = Bach Werkverzeichnes, or catalog of Bach's works.

Score: [Bach Chorale BWV 66.6](https://www.bach-chorales.com/BWV0066_6.htm)

Recording: [The Choir and Orchestra of the J. S. Bach Foundation, Rudolf Lutz, conducting.](https://www.youtube.com/watch?v=qFlTRAhCav8) The organist improvises the organ parts at the fermatas; you will not see that notated in the score.

We will work with this because it is the shortest chorale Bach wrote and thus the easiest to understand. We will sing through this piece several times in class, so I encourage you to find a voice part or two and sing them along with the choir until you are very familiar with it. This piece has some strange and wonderful moments. 

Questions to think about:

- What key is this chorale in?
- If multiple keys, where are the transitions?
- Where does the soprano line behave weirdly?

Readings: [music21 User's Guide](http://web.mit.edu/music21/) 

- [Chapter 4 \[Streams I\]](https://www.music21.org/music21docs/usersGuide/usersGuide_04_stream1.html): provides a basic introduction to Python lists and Streams. It also introduces getElementsByClass() and getElementsByOffset(), which were not covered in class.
- [Chapter 5 \[programming review, Lists of Lists\]](https://www.music21.org/music21docs/usersGuide/usersGuide_05_listsOfLists.html): a refresher for people whose work with nested data structures is a bit rusty.
- [Chapter 6 \[Streams II\]](https://www.music21.org/music21docs/usersGuide/usersGuide_06_stream2.html): Stream Recursion, Hierarchies, and Flattening.
- [Chapter 26 \[Iterations, Filters, and getContextByClass\]](https://www.music21.org/music21docs/usersGuide/usersGuide_26_iterators.html): advanced techniques in moving through a Stream and finding the elements you want. Optional, but helpful for PSet 3

This introductory video concerns a major aspect of Music Information Retrieval that shows how the steps of going from Sound to Score present problems related to music theory and analysis: 

{{% resource_link "2d23844d-d0fb-414e-8d90-0f7069d3a0dd" "Video 9a: Music Information Retrieval (MIR): Sound to Score and Music Theory" %}}

Questions for Sound to Score:

- For which of the following steps in the Sound to Score process are Fourier transforms most useful? 
    - Group of answer choices
    - Layout Score to Output
    - Virtual Score to Layout Score
    - Pitches to Tempo Estimation
    - Time Domain to Frequency
- What is one way *using an example from the video* that music theory/musicology can learn/gather data from the MIR process?
- Describe one way *not used as an example in the video* that you believe that knowledge from music theory/musicology could be used to verify/correct data from a MIR Sound to Score process to send the process back to a previous step. Specify what part of the pipeline the data would be used at and what part of the pipeline the process might be sent back to.

The most important representation format for CWMN today is MusicXML. Video 9b provides a brief introduction to how MusicXML works:

{{% resource_link "7ff2fefb-564f-4e21-8bcb-d0bf794a0564" "Video 9b: Introduction to MusicXML" %}}

Michael Good, the inventor of MusicXML, sat down with me over Zoom to talk about the creation of MusicXML:

{{% resource_link "d987b47d-6c02-4c04-8e59-d867a46c7bc0" "Video 9c: Interview with Michael Good on MusicXML" %}}