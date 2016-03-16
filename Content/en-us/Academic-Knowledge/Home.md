<!-- 
NavPath: Academic Knowledge API
LinkLabel: Overview
Url: Academic-Knowledge-API/documentation/overview
Weight: 100
-->

# Academic Knowledge API

Welcome to the Academic Knowledge API. With this service, you will be able to interpret user queries for academic intent and retrieve rich information from the Microsoft Academic Graph (MAG). The MAG knowledge base is a web-scale heterogeneous entity graph comprised of entities that model scholarly activities: field of study, author, institution, paper, venue, and event. 

The MAG data is derived from mining pages from the Bing web index as well as an in-house knowledge base from Bing. As a result of on-going Bing indexing, this API will contain fresh information from the Web following discovery and indexing by Bing. Based on this dataset, the Academic Knowledge APIs can enable a knowledge-driven, interactive dialog that seamlessly combines reactive search and proactive suggestion experiences, rich research paper graph search results, and histogram distributions of the attribute values for a set of papers and related entities.

For more information on the Microsoft Academic Graph, see [http://aka.ms/academicgraph](http://aka.ms/academicgraph).

## Features
The Academic Knowledge API consists of three related REST endpoints:  
  1. **interpret** – Interprets a natural language user query string. Returns annotated interpretations which can enable rich search-box auto-completion experiences that anticipate what the user is typing.  
  2. **evaluate** – Evaluates a query expression and returns Academic Knowledge entity results.  
  3. **calchistogram** – Calculates a histogram of the distribution of attribute values for the academic entities returned by a query expression, such as the distribution of citations by year for a given author.  

Used together, these API methods allow you to create a rich semantic search experience. Given a user query string, the **interpret** method provides you with an annotated version of the query and a structured query expression, while optionally completing the user’s query based on the semantics of the underlying academic data. For example, if a user types the string *latent s*, the **interpret** method can provide a set of ranked interpretations, suggesting that the user might be searching for the field of study *latent semantic analysis*, the paper *latent structure analysis*, or other entity expressions starting with *latent s*. This information can be used to quickly guide the user to the desired search results.

Based on the above interpretations, the **evaluate** method can be used to retrieve a set of matching paper entities from the academic knowledge base, and the **calchistogram** method can be used to calculate the distribution of attribute values for a set of paper entities which can be used to further filter the search results.        


## Getting Started 
To quickly go through the basic functionalities of the Academic Knowledge API, please refer to the three methods (**[interpret](InterpretMethod.md)**, **[evaluate](EvaluateMethod.md)**, and **[calchistogram](CalcHistogramMethod.md)**) in this documentation.  Please note that in the examples provided, the REST API calls have not been URL-encoded in order to improve readability in this documentation. Please be sure that your code applies URL-encoding to your requests.  


