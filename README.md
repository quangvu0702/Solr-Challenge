# Solr Challenge

### I designed this Challenge for me: Learn Solr in Depth in 4 weeks!!

### Prerequisites
* Basic level of Java.
* At least one year in software engineer.

## Index
 - **[Week 1 - Introduction](https://github.com/quangvu0702/Solr_challenge/new/master?readme=1#week-1---introduction)**
 - **[Week 2 - Core Solr capabilities](https://github.com/quangvu0702/Solr_Challenge/blob/master/README.md#week-2---core-solr-capabilities)**
 - **[Week 3 - Taking Solr to the next level](https://github.com/quangvu0702/Solr-Challenge/blob/master/README.md#week-3---hands-on-solr)**
 - **[Week 4 - Write a plug-in for solr]()**
<br>

## Week 1 - Introduction
- Videos:
  * [Solr 101](https://cognitiveclass.ai/courses/introduction-to-solr) (about 1 hour)
     - Videos only. We will practice later.
     - You don't need to remember everything. Just view the videos and get the concept of solr.
- Reading: [Part 1 Meet Solr. One chapter per day.](https://livebook.manning.com/book/solr-in-action/about-this-book/)
  * Chap 1 Introduction to Solr: (nearly 2 hours)
    - text-centric, read-dominant, documentoriented, and flexible schema
    - Solr use cases.
    - Key components of Solr.
  * Chap 2 Getting to know Solr: (nearly 1 hour)
    - It time to read. Don't code.
    - Sorting, paging, and results formatting.
  * Install solr and index sample: (about 1 hours)
    - Only work on Exercise 1.
    - [I install solr 7.7](http://lucene.apache.org/solr/guide/7_7/solr-tutorial.html#solr-tutorial)
    - [Index data in solr](http://lucene.apache.org/solr/guide/7_7/solr-tutorial.html#index-the-techproducts-data)
    - [Try basic search](http://lucene.apache.org/solr/guide/7_7/solr-tutorial.html#tutorial-searching)
  * Chap 3 Key Solr concepts: (about 2 hours)
    - Fundamental problem search engines are solving 
    - The basic structure of Solr’s internal index
    - FUZZY/EDIT-DISTANCE SEARCHING, PROXIMITY SEARCHING
    - How Solr calculates scores for matching queries to the most relevant documents
  * Chap 4 Configuring Solr: (nearly 2 hours)
    - How queries are executed.
    - Params: q, fq, sort, fl, df, wt, start, rows
    - Components: query, facet, more like this, highlight, stats, debug.
  * Chap 5 Indexing: (about 3 hours)
    - Documents, id, indexed fields, 
    - Fields, field types, and schema design.
    - Fields, dynamic fields, and copy fields
    - (Optional) [solr-field-types](http://lucene.apache.org/solr/guide/7_7/solr-field-types.html)
  * Do exercise: (nearly 1 hour)
    - [Do Exercise 2](http://lucene.apache.org/solr/guide/7_7/solr-tutorial.html#exercise-2)
    - [Update and delete data](http://lucene.apache.org/solr/guide/7_7/solr-tutorial.html#exercise-3)
  * Chap 6 Text analysis: (about 2 hours)
    - The analyzer, tokenizer, and chain of token filters.
chain of token filters.
- Coding: [Finish solr tutorial](http://lucene.apache.org/solr/guide/7_7/solr-tutorial.html#solr-tutorial)

## Week 2 - Core Solr capabilities

- Reading: [Part 2 Core Solr capabilities](https://livebook.manning.com/book/solr-in-action/about-this-book/)
  * Chap 7: Performing queries and handling results (about 4 hours)
    - Request handlers
    - Parameters
    - Finding, ordering
    - filter query, query
    - eDisMax
  * Chap 8: Faceted search (about 2 hours)
    - facets
    - field facet
    - range faceting
  * Chap 9: Hit highlighting (option)
  * Chap 10: Query suggestions (about 1 hour)
    - Four general scenarios
    - Type-ahead suggestions
  * Chapter 11: Result grouping / field collapsing (about 1 hour)
    - sdfsdf
  * Chapter 12: (Optional)
  * Chap 13, 14, 15: (Optional)
  * Chap 16 Mastering relevancy: (3 hours)
    - Debug result
    - Per-field boosting, per-term, payload boosting, function boosting.
    - Personalized search.
    - distance boost
  
## Week 3 - Hands-on Solr
 - Vides:
   - [Solr 101](https://cognitiveclass.ai/courses/introduction-to-solr) (about 1 hour)
     - Videos only. We will practice later.
   - [Rebuilding Solr 6 examples: layer by layer - Alexandre Rafalovitch, Search Stack Solutions](https://www.youtube.com/watch?v=lc6krl8iC9o) (about 1 hour)
 
 - Hands-on:
   - [apache-solr-intro-to-examples](https://dmidma.wordpress.com/2017/03/31/apache-solr-intro-to-examples/) (about 2 hours)
     - Goals: start Solr -> pick a .csv file -> create schema.xml -> query -> analyzer.
     - Note: all the files you need [here](https://github.com/quangvu0702/Solr-Challenge/tree/master/collection1)
   - Indexing:
     - Goals: learn how to design schema.
     - Key words: indexed, stored, type, required, field, dynamic_field
     - Reread [chapter 5: indexing](https://livebook.manning.com/book/solr-in-action/chapter-5)
     - [Download data](https://www.manning.com/downloads/683)
     - Implement EXAMPLE MICROBLOG follow instructions in chapter 5: reload core and test the effect of the code you change, modify tweets.xml to the right format with the changed code.
     - [All code you need are here.](https://github.com/quangvu0702/Solr-Challenge/tree/master/microblog)
   - Text analysis:
     - Goals: learn how to use analizer.
     - Key words: tokenizer, analizer, stop words.
     - Reread [chapter 6: indexing](https://livebook.manning.com/book/solr-in-action/chapter-6)
     - Add analizer to EXAMPLE MICROBLOG.
     - [All code you need are here.](https://github.com/quangvu0702/Solr-Challenge/tree/master/microblog-chapter6)
   - Query:
     - Goals: learn how to query solr to get the result we want.
     - Key words: 
     - Reread chapter 7 and 8
     - Implement EXAMPLE RESTAURANT follow instructions in chapter 8
     - [All code you need are here.](https://github.com/quangvu0702/Solr-Challenge/tree/master/restaurants)
     
## Week 4 - Write a plug-in for solr

# Reference:
- http://web.stanford.edu/class/cs224w/?fbclid=IwAR2BkOohuJW-DMOJ5nUeafLAdOEgrtHVijc2NF7XJcyCrjMXVCQ9akgysXA
- http://snap.stanford.edu/class/cs224w-videos-2017/
- https://cwiki.apache.org/confluence/display/SOLR/DIHQuickStart
- https://www.slideshare.net/arafalov/rebuilding-solr-6-examples-layer-by-layer-lucenesolrrevolution-2016
- https://www.youtube.com/watch?v=jNK2bNINSGM&list=PLCoJWKqBHERu9Fe0W12D7XKwGT2eoJJNU
- https://github.com/o19s
