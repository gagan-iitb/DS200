# DS200 (Architecture for Management of Large Datasets)

This is the course web-page for Architecture for Management of Large Datasets being taught at [IIT Bhilai, India](https://www.iitbhilai.ac.in/index.php) in the Monsoon Semester of 2021.

<br> Course Instructor: [Dr. Gagan Raj Gupta ](https://www.iitbhilai.ac.in/index.php?pid=gagan)

Other Instructors: [Dr. Soumajit Pramanik](https://www.iitbhilai.ac.in/index.php?pid=soumajit), [Dr. Subhajit Sidhanta](https://iitbhilai.ac.in/index.php?pid=subhajit)

Teaching Assistant: Muttareddygari Sreechakra

Motivation
----------
Over the past few years, we have seen the emergence of "big data": disruptive technologies that have transformed commerce, science, and many aspects of society. These developments are enabled by infrastructure that allows us to distribute computations across hundreds or even thousands of commodity servers.

* Getting data is becoming easier day by day, but we have _too much_ to analyze (e.g. web, transactional data, text)
* Data has _errors_ of various types (missing, incorrect etc.), is _incomplete_ and is _hard to clean_ (e.g. user reviews/ratings, distorted images) 
* Data is usually _high-dimensional_ (involving lot of columns or features) (e.g. text, images, videos, graphs)
* Data usually has _complex correlations_ and i.i.d. assumptions don't always work very well (e.g. graph data, time-series data) 
* Data is being generated at a _great speed_ and it is too _expensive to store_ all of it (e.g. user or machine transactions, queries)

__In this course, we want to learn how large datasets are maintained and analyzed. If a single computer is not enough, how do we use multiple computers (even datacenters) to analyze large datasets? How do we make programming easy for data analysis and ML?__

One key breakthrough that makes this all possible is the development of abstractions for data-intensive computing that allow programmers to reason about computations at a massive scale, hiding low-level details such as synchronization, data movement, and fault tolerance.

This course provides an introduction to big data infrastructure, starting with MapReduce, the first of these datacenter-scale programming abstractions. The Hadoop implementation of MapReduce lies at the core of an application stack that has gained widespread adoption in both industry and academia. A major focus of this course is algorithm design and "thinking at scale", applied to a variety of domains: text, graphs, relational data, etc. We will also cover a few next generation systems that are vying to replace MapReduce as the de facto big data processing platform of tomorrow.

Course Objectives
-----------------
* Motivate the need for managing large datasets. 
* Develop the architectural requirements for a data store (lake)
* Introduce various distributed programming models and abstractions
* Explain new paradigm of __algorithm design__ with MapReduce for handling large datasets 
* Introduce __streaming algorithms__ for processing streaming data
* Provide hands-on experience to students in analyzing datasets in diverse fields __(Industry 4.0, NLP, Graphs, Networks, Bio-informatics, Time-series)__
* Understand the software architecture

Pre-requisites
--------------
* Basic knowledge of Python (most assignments will be based on Python)
* Knowledge of basic computer science principles and skills

Tentative Course Outline
-------------------------
|Lec #| Date| Topics covered in class | Text Book Reference, readings |
| --- | ------------| ----------- | -------- |
|1| Sep 28 | Large Datasets Examples; Data-center Architecture; Important of Analysis; Requirements on Architecture for Managing Large Datasets;  How would you analyze large dataset?: Sequential vs. Parallel Programming;  Higher levels of Abstraction for Parallel Programming: Datacenter is new computer; Data Intensive and Data Parallel Computing; MapReduce introduction |  |
|2| Sep 30 | Von-Neumann Model and current computers; Memory Hierarchy; Storage Technologies; Parallel Reads and Writes; Reliability and Cost Tradeoff with distributed file systems, latency and throughput; External Memory Algorithms: External Merge Sort||
|3| Oct 1 | Reliability Cost Tradeoff review; Streaming Model Introduction; Paralel Computing Models: synchronization; PRAM model: Computing Minimum with N/2 Processors via Tournament Method, Correctness, Solving with P<N/2 processors; BSP model; Map Reduce Explained; Demo of scalability via Map-Reduce on word-count problems||
|4| Oct 5 | Map Deep Dive; Programming Paradigms: Declarative, Functional; Generators; Lazy evaluation; Parallel Map on multi-core machines; Out of Order Execution||
|5| Oct 7 | Reduce Deep Dive; Aggregation||
|6| Oct 8 | Map-Reduce; Optimization: Combine construction of Map Reduce; ||
|7| Oct 12 | Filtering patterns: Data cleaning, Bloom Filters for Set Membership, Top 10, Distinct items | |
|8| Oct 14|  Pipelining, Chaining | |
|9| Oct 21| More patterns, Exam 1 Review/Prep| | 

Meeting Times
-------------
* Lectures (Tue, Thr 11:30 a.m., Friday 4:00 p.m.) on https://iitbhilai.webex.com/meet/Conference_1

Books/References/Practice materials
-----------------------------------
* Course Textbooks
  * Hadoop: The Definitive Guide, 4th Edition : https://www.oreilly.com/library/view/hadoop-the-definitive/9781491901687/
  * Mastering large datsets with python : https://www.manning.com/books/mastering-large-datasets-with-python
  * Data-Intensive Text Processing with MapReduce : https://lintool.github.io/MapReduceAlgorithms/
  * Map-Reduce Design Patterns : https://www.oreilly.com/library/view/mapreduce-design-patterns/9781449341954/
  
* Handouts (short notes on various important topics)
* Sample code snippets will be posted in the Handouts section for students to practice data analysis programming
* Useful datasets will also be provided for practice

Similar Courses
----------------
* https://people.eecs.berkeley.edu/~istoica/classes/cs294/15/
* http://lintool.github.io/UMD-courses/bigdata-2015-Spring/overview.html
* https://www.cs.utexas.edu/~dfranke/courses/2018fall/cs378-BDP.htm
