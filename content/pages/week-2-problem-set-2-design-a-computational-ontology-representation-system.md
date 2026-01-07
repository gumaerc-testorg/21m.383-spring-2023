---
content_type: page
description: Problem set is described in detail.
draft: false
title: 'Week 2: Problem Set 2: Design a Computational Ontology and Representation
  System'
uid: 3614961d-7dab-4087-87e6-3550304f30ac
---
In groups, design a computational **ontology** and representation system for a type of music, a facet of music, a relationship between music and something else, or basically ANYTHING music-related.

**Point 1:** Submit a description of the repertory that you are working on and 2–3 sentences on what difficulties it entails and what is important to encode about it that wouldn’t be the case for Common Western Music Notation. (10% of the grade is getting this in on time).

**Point 2:** The remaining 90% will be decided by a write-up (approx. 4–10 pages, about 1000–1800 words) that includes the points discussed below:

- (8%) Originality of the repertory and of the problem to be solved.
    - *Half of this score will be based on your argument about the originality, and half my subjective impressions of the originality.*
- (10%) Impact of the proposed work and what it might accomplish.
    - *Almost all of this score will be based on your argument of the impact.*
- (72%) Design and completeness of the ontology (representational system). Effectiveness in solving the problem, broken down as the following components:
    - (10%) Description of the ontology/representation system (prose)
    - (12%) Quality and completeness of the system and choices of how to represent it in a file
    - (8%) Examples of the encoding of particular elements
    - (10%) Having a clear taxonomy/meronomy of the elements of the representation, including precise definitions of terms used
    - (10%) A “Hello World” encoding of a very short piece/problem/etc. as a file that could in theory be parsed (if a parser existed)
    - (5%) Citation of two other representational systems that gave ideas (or dead-ends) towards this solution (including authors’ names, links, and publications/official specifications, all collected in a bibliography at the end)
    - (10%) Quality of writing
    - (5%) Effective examples explaining the ontology/representational system, referred to with figure numbers, captions, and references in the text
    - (2%) Description at the end of the write-up of what each person on the team contributed

You should *not*

- Implement a parser, or software for working with or analyzing the repertory, or reach analytical conclusions. That is not this assignment. You must, however, create an encoding that would make such software possible, at least in theory.
- Use any easy-to-read format (e.g., PDF, Google Docs, MS Word, Jupyter Notebook, PowerPoint, etc.) that best explains your work.

If you need to encode Western classical notes, pitches, durations, etc. at any point, you should assume that that part of the problem is solved. For instance, “An *X-widget* is a mapping of an *X-factory* to a list of CWMN notes (encoded somehow) that sound at the same time the *X- controller* performs her first event.” Again, do not waste space implementing yet another encoding system for common western classical notes—you will not get credit for it, and it will just waste time.

**Ideas of repertories to get you started** (note: taking something directly from this list will score lower on originality):

- Jianpu, or numbered musical notation
- Turntablist transcription method, or “scratch notation”
- California Indian music and ceremony
- Unmeasured preludes of Elizabeth Claude-Jacquet de la Guerre or Louis Couperin
- Aleatoric, or “chance” music (Cage, Brown, and many, many others)
- Frequency-based music (e.g., Stockhausen’s *Studie II*, music using non-equal temperament tuning systems)
- Graphic notation (e.g., Lachenmann’s *Pression*)
- Senegalese drum notation
- Video game music’s connection between music and event
- Connecting an arrangement’s notes to the original etc.

**Some ways that you might go about solving the problem:**

1. Familiarizing yourself with your repertory
    - Find a few relevant recordings of the pieces (if they exist) or scores (if they exist). Think about how the current physical notational system organizes relevant information and how that information relates to the audible manifestation of the music. List the basic structural units of the music. How are they organized?
    - Similarly, what types of instruments, techniques, or equipment are needed to perform the music?
    - How do people who are practitioners of the repertory (performers, composers, listeners) talk about the music and how will this affect the ontology (terms, relationships, representation) you use?
2. Research utility and impact
    - What type of analysis might researchers be interested in carrying out on your repertory? Who would be the various groups affected by the outcomes of that research and what might those effects be?
    - Similarly, think about the traditions and cultural considerations associated with your repertory, as well as the skills and limitations of the researchers and musicians working with the repertory. For instance, is the music in your repertory associated with a primarily oral tradition? Would the musicians or researchers interacting with the repertory be classically trained? Is a competence with digital signal processing necessary for the performance of the works comprising your repertory? etc. Explain how your implementation would take into account these factors.
3. Designing a digital notational schema
    - Choose a language(s), file type(s), and any associated software and add-ons that would be necessary for your implementation to be useful for score analysis, notation editing, performance, etc. Implement a bit of the notational system so we can see how it works. Document this system.
    - Map out a class hierarchy to organize the relevant structural units of your system. Think about the attributes associated with each object and the methods that might be involved with each. *(Just in case you were still wondering why 6.009 is a prerequisite for the class!)*
    - Provide some basic documentation that gives an overview of how your encoding would interact with existing software systems (or hypothetical ones that might be developed) and if your system interacts with other encodings (such as CWM notes, etc.) how the two systems work together.
4. Considering the efficiency, overhead, and reuse of your encoding
    - What types of pre-existing notations, encoding standards, languages, or interfaces could be used to implement your schema? Are there any particular advantages/disadvantages to using these?
    - What is the means by which your repertory could be stored and accessed? Think a little about file size, but more about transportability and compatibility with existing file types, programs, and software suites necessary for analysis, viewing, and playback.

**Common caveats to watch out for:**

- Did you remember to encode some of your music/repertory?
- Do your figures have captions and numbers and are they referred to in the prose text?
- Does the system provide enough information that two people could have a fighting chance of encoding the same piece/event in the same (or basically similar) way?
- Can your encoding, in theory, be decoded to represent the same piece/event?