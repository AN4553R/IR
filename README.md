# Motivation
Information retrieval (IR) is finding material (usually documents)
of an unstructured nature . . . that satisfies an information need
from within large collections (usually stored on computers).

> Basic assumptions of IR
+ Collection: Fixed set of documents
+ Goal: Retrieve documents with information that's relevant to the user's information need and helps the user to complete a task

## Description
### Boolean Retrieval Model

The Boolean model of information retrieval (BIR) is a classical information retrieval (IR) model and, at the same time, the first and most adopted one. It is used by many IR systems to this day

In the Boolean retrieval model we can pose any query in the form of a Boolean expression of term i.e., one in which terms are combined with the operators and, or, and not.

> Basic Assumption of Boolean Model
+ An index term is either present(1) or absent(0) in the document
+ Queries are Boolean combinations of index terms.
+ X AND Y: represents doc that contains both X and Y
+ X OR Y: represents doc that contains either X or Y
+ NOT X: represents the doc that do not contain X

### An example information retrieval problem

`Brutus AND Caesar AND NOT Calpurnia`

Suppose you wanted to determine which plays of Shakespeare contain the words Brutus and Caesar and not Calpurnia. One way to do that is to start at the beginning and to read through all the text,

The simplest form of document retrieval is for a computer to do this sort of linear scan through documents. This process is commonly referred to as GREPPING through text

+ The way to avoid lineraly scanning the text for each query is to `index` the documents in advance.

+ Suppose we record for each document whether it contains each word out of all the words that may be used.

+ The result is a binary term-document `incidence matrix`.

+ Terms are the indexed units. They are usually words.

### The included process

+ Documents to be indexed.

+ Token stream

+ Modefied tokens (Stemming).

+ Indexer (incidence matrix).

![one](Screenshot%20(93).png)
![two](Screenshot%20(94).png)
![three](Screenshot%20(95).png)
![four](Screenshot%20(96).png)
