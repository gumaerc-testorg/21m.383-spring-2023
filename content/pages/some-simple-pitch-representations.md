---
content_type: page
description: Preparation for problem set 1
draft: false
title: 'Week 1: Class 3: Some Simple Pitch Representations'
uid: f0e64821-65ef-41b7-9dba-a1d9bd7cdfc9
---
The first problem set is (no surprise) on pitch representation and manipulation. We will for much of the assignment consider five different pitch representations:

1. Frequency (as a float)
2. MIDI/Pitch Space number (as an int/float)
3. String of pitch name (as a str)
4. String of pitch name with octave number (as a str)
5. Pitch class (as an int)

**Frequency** is pretty self-explanatory. 440.0 = 440 hertz  

**MIDI number** is a mapping of (essentially) piano keys to numbers defined so that 60 = middle C. So 61 = C# but it also = Db. 62 is D but also Cx (double sharp) and also Ebb.  etc.  **Pitch Space** is basically exactly the same as MIDI number except that it's a float (60.0 = middle C) so there could be pitches between C and C#. Also, MIDI numbers are constrained to be between 0 and 127, while pitch space numbers are unbounded (so they could be negative or 99999, etc.).

String of **pitch name** is a string like "C#" or "F". (In the problem set we will explain why many of us in computational music analysis have chosen to **call B-flat not "Bb" but instead "B-"**.) C double-sharp could be "Cx" but most programmers write out "C##" instead. G double-flat would thus be "Gbb" or "G--". There are notes with [Triple Flats](https://dictionary.onmusic.org/terms/3683-triple_flat#:~:text=This%20term%20refers%20to%20an,%E2%99%AD%29%20symbols%20preceding%20the%20note.&text=Most%20musicians%20%28professional%20or%20amateur,in%20their%20entire%20musical%20career.) and [Triple Sharps](https://dictionary.onmusic.org/terms/3687-triple_sharp) and even Quadruple accidentals but they're really rare but occasionally useful (but a stickler might expect your software to work if it encountered them).

String of **pitch name with octave** number is a string like "C#4" or "B2" or "G-0" where middle C is C4, and the B below that is B3 (and C4's enharmonic is B#3, not B#4). Note that in this case, negative octave numbers cannot be represented because is "D-2" a Db in octave 2 or a D-natural in octave -2? Thankfully there aren't instruments that go down that low.

Here's [a little chart showing how these representations interrelate](https://audiodev.blog/midi-note-chart/midi-note-chart.jpg).

**Pitch class** is like a MIDI number but octave is not taken into account and is used primarily in twentieth-century and atonal music. So 0 = any C (and any Dbb or B#), 1 = C#/Db, 2 = D, etc. You'll see Pitch class used a lot in the Tymoczko reading.

As you've no doubt thought through by now, each of these representation systems works better for some things and worse for others. Thus a good portion of the PSet will be spent on converting between different representation systems.