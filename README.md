# Lecture Notes for Data Engineering in Spring 2015

## Lecture 1

STORM FRAMEWORK (TWITTER)


*SOCIAL NETWORKS
*DATA ANALYTICS
SAMPLING: NARROWING DOWN LARGE DATA SETS TO RELEVANT REASONABLE SETS THAT COULD BE ANALYZED TO ANSWER SUPPORT A HYPOTHEISIS OR  ANSWER A RESEARCH QUESTIONS
BIG DATA IS NOT ALWAYS ABOUT SAMPLING CAUSE WE CAN COMPUTE EVERY THING WITH THE POWER OF COMPUTING 
*STORAGE: NOSQL (PROBLEMS WITH DATA SCHEMA CHANGES IN SQL) NOT FLEXIBLE
          NOSQL ARE NOT GOOD WITH ARBITRARY QUERIES
          NOSQL: DOCUMENT, GRAPH, KEY-VALUE STORES,COLUMNAR
*DATA MODELING IS WICKED HARD :) PROBLEM WITH BIG DATA SITUATION E.G. STRUCTURE OF DATA CHANGES BECAUSE THE CURRENT DOES NOT ANSWER THE QUESTION (SOLUTION MIGRATION EXPENSIVE BUT DOABLE)
*DATA COLLECTION + CLEANING (COVERED MORE IN OTHER COURSE) WHAT IS IN CLEANING: IT IS IN THE FORMAT I NEED? NORMALIZATION?

MORE ABOUT TWITTER:
SOME TWITTER CLIENTS SEND TWEETS THAT ARE NOT UTF-8 EVEN THOUGH IT TAGS THEM AS UTF-8 WHEN WE USE JSONS PARSERS WE GET TWEETS THAT HAVE MESSY ENCODINGS

*INFOVIZ:
D3 jscript framework for visualization on the browser
TABLOAR
EXCEL

THE DATA LIFE CYCLE:

WHAT IGNITES THE LIFE CYCLE IS A QUESTION --> CURATION/TRIAGE (FINDING THE RIGHT SOURCE NARROWING DOWN AKA CURATION/TRIAGE)
COLLECTION/GENERATION --> CLEANUP --> STORAGE --> PROCESSING/ANALYSIS --> QUERY/VISUALIZE/ACT

THE CYCLE REPEAT (ITERATIVE): AS THE LAST PHASE TRIGGERS NEW QUESTIONS WHICH TAKES TO PHASE 1

HTTP (REQUEST RESPONSE CYCLE) MORE ON THURSDAY

## Lecture 2

Git scales well as version control system

Git is a distributed version control system

Ancient version control system: SVN,CVS are not distributed

Notes from Markdown presesntation:

Two Types Markdown:
Standard Markdown (SM)
Github Flavored Markdown (GFM)

Headers up to six

Italic: *this* _this_
Bold: **this** __this__

two spaces or two enters for a new line for a new paragraph

iawriter: convert markup to some pdf or doc (github convets to HTML)

Markdown resource: daringfireball.net

HTTP + RESFUL Notes:

GET

POST

DELETE (Security risk as clients might delete server content)

PUT

Handler: A separate entity not part of the webserver it handles request passed by the webserver

Static webpages (request): usually the webserver passes an index.html file and the client's browser parses the html and display to the user

Static web pages: In many cases a single webpage request triggers another requests not the the initial server only it could be to other servers (images loaded via other requests *the URL is embedded in the HTML*)

Amazon Example: Amazon does not return a static index.html in fact the content generated dynamically from services that tailor content based on the user's data in their network (ads are somewhat relevant to your browsing)

Protocol: what messages format and order of messages (HTTP protocol) ALL TEXT REQUIREMENTS DOCUMENT FOR IMPLEMENTING APPS USING HTTP

HTTP VS. RESTFUL?  Architecture (design pattern) and is appraoch for building a service based application while HTTP is a protocol

*Resources: URI (URL subset of URI, URI are more generic)
*CRUD (CreateReadUpdateDestroy)

EX:

/users (resource for all users) or /users/{id} (particular user)

GET -Read (read current state of a resource)
POST -Create (data)
PUT -update
DELETE -Destroy that user

Limit of URL: 1024 characters

Can POST used to be read:

TWITTER EXAMPLE (SEARCH API ENDPOINT): with a get request there is a limit to the URL so searhc parameters are limited 1024 therefore we subsitute POST and pass the search parameters as updates.

SINATRA: WEBSERVICE FOR RUBY (NOT USED FOR PRODUCTION)

Best Practice: put your version in your protocol (URL)

The Contact Example (RESTFUL With Ruby) Questions:
*Database? where to store
*IDs? what does the new contact get as an ID (Prof used integers and increments)
*What Input?
*What output?
*Error Handling? (requests half baked)


