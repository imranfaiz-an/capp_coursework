# Relevant CAPP CS Coursework (code available on request)
This repository lists some of the programming assignments that I worked on as part of the core CAPP curriculum.

---


## Computer Science with Applications II - CAPP 122 (Winter 2026)

- Congressional Hearings (APIs)
  - For this assignment I worked with a live API based on the official [congress.gov](https://www.congress.gov/) API. I wrote a module to download, cache and load the API data, after converting the JSON data to a CSV file I do basic word count analysis using ngrams. To finish I wrote CLI to allow users to get a breakdown for the most used words in congress on a given day and to search for a word and get a count of how many times in total it has been heard in congressional hearings.
  - Libraries Used: HTTPX, pathlib
  - Topics covered: Caching API data, working with a real API, text analysis
- Scraping Chicago Parks (Web Scaping)
  - Built web scrapers to crawl [Chicago Parks](https://www.chicagoparkdistrict.com/parks) website, this assignment provided an introduction to inspecting HTML code for websites and how different divisions, ids and classes can be exploited to get to a specific part of the website and fetch that data (using cssselect and lxml.html libraries). Once I fetched all the data through crawls pf all webpages for indvidual parks, I cleaned the text using the re library and return the complete dataset as JSON.
  - Libraries Used: cssselect, lxml.html, re
- What's the News (Markov Model & Hash Tables)
  - Developed a text modeling system using Markov models. This assignment introduced key CS concepts like time complexity and how to implement O(1) data structures to help reduce compute time. I implemented a Hash Table data structure with [linear probing](https://en.wikipedia.org/wiki/Linear_probing) from scratch. The Hash Table had ```__setitem__ & __getitem__``` methods defined where I was explicitly handling collision cases and rehashing the entire table if the length exceeded a certain threshold. Once the Hash Table was implemented, I implemented the Markov model (learning algorithm) that takes text as input and return the probabilty that the text comes from a given source.
  - Topics Covered: time complexity, hash tables, Markov models  
- EPA Analysis (Geospatial Data Analysis)
  - I worked with QuadTree data structure for this assignment and worked on optimizing the function to check if one geospatial data structure contains another (e.g., points within polygons). Using bounding boxes around polygons and checking whether the point is within the bounding box before checking within a polygon, I was able to reduce the total computation time significantly. The dataset used was the [US Environmental Protection Agency's Facility Registration Service (FRS)](https://www.epa.gov/frs/epa-frs-facilities-state-single-file-csv-download) facilities which were the geospatial points and census tracts which served as the polygons for the spatial joining. 
  - Libraries Used: Shapely, pyshp
  - Topics covered: geospatial joins, recursion, quadtrees
- Data Linkage and Cleaning (String Matching Algorithm Optimization)
  - (In Progress)
  - Libraries Used: Jellyfish, re
- Trade Graphs (Network Analysis & Graphs)
  - Woked with graphical data using the [2024 UN Trade Data](https://comtradeplus.un.org/). Wrote function to calculate stats like imports/exports within two countries and simulated trade wars and trade embargos between countries by manipulating the edges in the digraph using the [NetworkX library](https://networkx.org/en/).
  - Libraries Used: NetworkX
 
---

## Computer Science with Applications I - CAPP 121 (Fall 2025)
This course covered the basic of python programming like data structures, control flows, iterations, oop, recursions and provided an introduction to numpy and pandas. After each module I worked on a programming assignment related to one of the aforementioned core concepts.

Programming Assignments:
- [Modelling Epidemics](https://classes.cs.uchicago.edu/archive/2022/fall/30121-1/pa/pa1/index.html) (Intro to Python Programming)
  - Overview: This assignment introduced basic python concepts and skills. For this assignment I wrote code simulate a simplified version of the SIR epidemic model. The model quantified how an infection spreads through a city.
  - Topics covered: control flows and basic python data structures (tuples, lists, integers, floats, booleans)
- [Schelling Model of Housing Segregation](https://www.classes.cs.uchicago.edu/archive/2024/summer/52072-1/assignments/proj1/index.html) (Functions)
  - Overview: For this assignment I modeled how a neighborhood with people of different identities segregates over time based on a simplified criterion which was a function of the neighbors each ```i, j``` indvidual had in 2D.
  - Topics covered: for/while loops, functions and their parameters, return statements
- [Analyzing Candidate Tweets](https://classes.cs.uchicago.edu/archive/2022/fall/30121-1/pa/pa3/index.html) (Dictionaries)
  - Overview: This assignment introduced dictionaries and their implementation in Python. I analyzed tweets from 4 four political parties in Britian and explored things like the most frequent terms mentioned in the tweets, frequent phrases, etc.
  - Topics covered: dictionaries, sets, dictionary and list comprehensions, k-mers
- [Polling Places](https://classes.cs.uchicago.edu/archive/2022/fall/30121-1/pa/pa4/index.html) (OOP)
  - Overview: The goal of this assignment was to practice designing and implementing classes and methods, and working with class instances. In this assignment, I wrote code to simulate the flow of voters through polling places and analyze the interplay the number of voting booths assigned to a precinct and the amount of time voters spend waiting in line.
  - Topics Covered: stacks, queues, classes, attributes (class vs. instance attributes), methods (e.g. dunder methods)
- [Visualizing Avian Biodiversity Using Treemaps](https://classes.cs.uchicago.edu/archive/2022/fall/30121-1/pa/pa6/index.html) (Recursions)
  - For this assignment I worked with the tree data structure in Python and used treemaps to visualize the frequency of bird sightings throughout the year.
  - Topics covered: trees, recursive lookups and binary searches
---

