# The Music Note Ontology
This repository contains material related to Music Note Ontology, as described in the article:

```text
Poltronieri, A., & Gangemi, A. (2021). The Music Note Ontology. In Proceedings of the 12th Workshop on Ontology Design and Patterns (WOP 2021), Online, October 24, 2021..
```
The Music Note Ontology models a musical note both as a
constituent element of the score, and as a musical object, i.e. as a realisation of 
the event represented by a score or symbolic notation. To do this, the proposed
ontology represents both the elements and the typical hierarchies of a score,
describing all its attributes. In addition, the ontology models the realisation of
a note, describing its physical characteristics in a given performance.
## Ontology Design

Ontology was modeled following the principles of [Ontology Design Patterns](http://ontologydesignpatterns.org/wiki/Main_Page) and 
aims at responding at the following competency questions: 

### Competency questions

| Id | Competency Question |
|----|---------------------|
| CQ1 | what is the name of a note? |
| CQ2 | what part of the score does a note belong to? |
| CQ3 | what are the dynamic indications referring to a note in the score? |
| CQ4 | what is the fundamental frequency of a note? |
| CQ5 | what are the different frequencies that make up the spectrum of a note? |
| CQ6 | what is the duration in seconds of a note, in a given performance? |
| CQ7 | how is the envelope of a note shaped? |
| CQ8 | what is the sound intensity of the notes played by a specific voice? |
| CQ9 | what is the MIDI pitch of a musical object having a specific frequency? |
| CQ10 | what is the decay time of the execution of a note? |
| CQ11 | which are the accidental of the notes present in a score part? |
| CQ12 | what is the duration in seconds of the notes played by a specific instrument? |
| CQ13 | what is the MIDI velocity of a played note in a given performance? |


## Ontology Modules

The Ontology is designed as the union of three different Ontology Design Patterns, namely:

### The Score Part Pattern
The hierarchy (i.e. the mereological structure) of a music score is described
by the [Score Part Pattern](https://purl.org/andreapoltronieri/scorepart).

### The Musical Object Pattern
The [Musical Object Pattern](https://purl.org/andreapoltronieri/) models the physical features of a musical note object, i.e. the execution of a note. 
Specifically, this pattern models the physical characteristics that can be extracted from the sound wave produced by an instrument playing a musical note

### The Music Note Pattern

The [Music Note Pattern](https://purl.org/andreapoltronieri/notepattern) models the symbolic note (as represented in a score
or in most of symbolic representation systems) and its attributes. Moreover, this
ODP aims to abstract over different music representation systems. This means
that it is possible to represent with this pattern music that was originally encoded
in other formats. To do so, the pattern proposed describes each symbolic notes
both by means of the standard music score notation and by using the MIDI
reference for each of the notes’s attributes.


## SPARQL Queries

For each of the Competency questions listed abouve we provide the relative SPARQL queries. 
All the SPAQRL queries are available in the folder [SPARQL_queries](https://github.com/andreamust/music_note_pattern/tree/main/SPARQL_queries)


## Cite

```text
@inproceedings{poltronieri2021musicnoteontology,
      title={The Music Note Ontology},
      author={Poltronieri, Andrea and Gangemi, Aldo},
      booktitle={Proceedings of the 12th Workshop on Ontology Design and Patterns (WOP 2021), Online, October 24, 2021.},
      journal={CEUR-WS},
      editor={Hammar, Karl and Shimizu, Cogan and Küçük McGinty, Hande and Asprino, Luigi and Carriero, Valentina Anita},
      year={2021},
      month={11}
}
```

## License

MIT License

Copyright (c) 2021 Andrea Poltronieri

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.