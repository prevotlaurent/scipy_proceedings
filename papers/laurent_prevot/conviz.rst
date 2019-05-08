:author: Laurent Prévot
:email: laurent.prevot@univ-amu.fr
:institution: Aix-Marseille Université, CNRS, Laboratoire Parole et Langage, France
:institution: Institut Universitaire de France, Paris, France
:institution: Institut Universitaire de France, Paris, France

:author: Nathan Vignal
:email: nathan.vignal@etu-univ.amu.fr
:institution: Aix-Marseille Université, CNRS, Laboratoire Parole et Langage, France

:author: Simone Fuscone
:email: simone.fuscone@univ-amu.fr
:institution: Aix-Marseille Université, CNRS, Laboratoire Parole et Langage, France
:institution: Aix-Marseille Université, CNRS, Laboratoire Informatique et Systèmes, France

:bibliography: conviz

----------------------------------------------------------------------------
Conversational Analytics and Visualisation with Modern Data Science Packages
----------------------------------------------------------------------------

.. class:: abstract

   We illustrate how to use and adapt generic data science packages for visualizing
   and analyzing conversational data sets. Our approach combines three levels of
   visualisation and analysis : at corpus level we present an interactive visualisation
   of the diversity of conversations, at conversation level, the temporal dynamics of
   relevant variables are presented as dialogic time series; Finally at deeper linguistic
   level we deal with distributions, clustering techniques and graph visualisation to strengthen
   insights into language structures. We argue that only such a multi-scale approach makes it
   possible to grasp conversational data sets without overlooking potential pitfalls.

.. class:: keywords

   Conversation, Data Science, Visualisation, Clustering, Time-Series analysis, Natural Language

Introduction
------------

We illustrate how to use and adapt generic data science packages (SciPy, Bokeh and Networkx)
for visualizing and analyzing conversational data sets. The conversations we consider in our
studies range from long unfocussed conversations between friends to short task-oriented dialogues.
We focus on speech modality our data set includes sometimes video data. Moreover most of what we present
can easily be adapted to other media such as instant messaging. Our goal is to provide a quantitative
and synthetic view of the data that is sufficiently rich and tailored to conversation to be relatable
to qualitative linguistic analyses. Our approach combines three levels of visualisation and analysis.
First, at corpus level we demonstrate an interactive visualisation the diversity of conversations and
provide a way to visually grasp the specificities of each conversational data set. Then, a conversation
level the temporal dynamics of relevant variables are presented as dialogic time series again in an
interactive visualisation. Finally a deeper linguistic level dealing with distributions (lexical
or higher level), clustering techniques and graph visualisation are used to strengthen insights into
language structures. We argue that only such a multi-scale approach makes it possible to grasp conversational
data sets without overlooking potential pitfalls (in research or application purposes).
For these purposes, we use a mostly unsupervised approach to our data sets in order to reduce the traditional
NLP bias for written genres. More precisely, in terms of base units we use both traditional “word-based”
segmentation and unsupervised segmentations (such as branching-entropy methods). Then, structures approximated
by sequences of either part-of-speech tagging, or again using cluster labels (acquired thanks contextual
distributions). Our last step is to compare sequences distribution we build graphs of sequences in which
distance between sequences (encoded on edges) is combined with frequencies (encoded on nodes). Finally,
we adapt standard data science APIs to match the structural specificities of conversational data sets.
The main specificities on data sets are (i) their different levels organisation (a corpus is made of
conversation, itself made of utterances) ; (ii) the importance of both the temporal dynamics of conversation
(time-series) and of distribution of items (being words or sequences, for example, of part-of-speech tags) ;
(iii) the dialogic nature of the data, most variables are need be handled as pairs (or more) of variables
since they belong to one participant and conversation involves at least a pair of them.


Corpus Level
------------

.. figure:: corpus.png
   :align: center

   General corpus comparison view. :label:`corpus`


   Corpus comparison view on specific variables. :label:`corpusVariable`


.. figure:: radar.png
   :align: center

   Corpus comparison on relevant conversational dimensions. :label:`corpusRadar`


:cite:`Yngve1970`



Session Level
-------------


Conversations as time series
============================


   Conversation view on specific variables. :label:`Session Variable`


Interpersonal dynamics
======================


Clustering conversations
========================


Linguistic Level
----------------

Lexical level
=============

Units / Tagging / Pattern extraction

\begin{figure}
    \centering
    \includegraphics{\}
    \caption{Lexical Frequency Distributions}
    \label{fig:my_label}
\end{figure}

.. figure:: lexical.png
   :align: center

   Lexical Frequency Distributions. :label:`lexical`

.. figure:: pos.png
   :align: center

   Syntactic categories Distributions. :label:`pos`



.. figure:: conversTag.png
   :align: center

   Conversational Tagging. :label:`converstag`


filled pause, feedback, dm, particles and the rest (distribution of an item)


Conversational Routines
=======================

.. figure:: graph.png
   :align: center

   Graph View of Extracted structures. :label:`graph`

:cite:`Pickering2004`

Related Work
------------

Well...

Ongoing and Future Work
-----------------------

that'all...


References
----------


