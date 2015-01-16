# Lecture Notes for Data Engineering in Spring 2015

## Lecture 1

-Storm (cluster based framework for big data similar to Hadoop but not intended for batch processing)

-Big Data Sampling: not always required. We can obtian and process massive amounts of data.

-NoSQL addresses schema changes well (it is felxible)

-NoSQL is not suitable for arbitrary queries

-Data Cleaning: Is it in a suitable format for processing and storage? Normalization?

-Data Visualization Technologies:

* InfoViz: jscript based
* D3: jscript based
* Excel based technologies

-__Data life cycle__:

Question/s --> Triage/Curation --> Collection and/or Generation --> Cleaning --> Storage --> Processing/Analysis --> Query/Visualize/Act

(it reapets last phase may introduce new questions which triggers a new cycle)

## Lecture 2

-Git is a version control system that scales well (distributed)

-Legacy version control systems (SVN, CVS, etc) are not distributed

-MarkDown: for a new line use double space or double enter (return)

-IA Writer: A Mac/iOS App that converts MarkDown to MS Office (may be pdf)

-MarkDown resource: daringfireball.net

-Webservices: Standardized way of integrating web applications using open standards (XML,JSON,SOAP,UDDI,WSDL,etc)

-Two web applications may be on different platforms, developed in different languages and technologies yet they are able to integrate and complement each other in business logic, data sharing ,etc seamlessly (via webservices)

-Webservices are meant to have applications talk to each other (they do not offer interfaces to users). However, 
developers may wrap webservices with GUI (browser based or desktop based) to enable users to make use of web 
services published by web applications

-HTTP vs. RESTful:
*HTTP: Is an application protocol (Textual Requirements for communication: Message formats, sizes and order, etc)
*RESTful: Is an Architecture Style/Design Pattern with constraints/guidelines used for creating web services which 
allow anything connected to a network to communicate with one another via HTTP protocol.

-HTTP Requests (messages):
*GET (Read)
*Post (Create)
*Put (Update)
*Delete (Destroy): Used to be disabled (security risks as clients may attempt to delete content handling must be 
imposed)

-Handler: A separate entity not part of the webserver it handles request passed by the webserver

-Static webpages request (via GET, it needs a URL): 
*usually the webserver passes an index.html file and the client (browser) parses the html and display it to the 
user
*In many cases a webpage request triggers another requests not limited to the initial server (images loaded via 
other requests -the URL is embedded in the HTML retrieved by the initial request-)
*Amazon Example: Amazon does not return a static index.html in fact the content is generated dynamically from 
services that tailor content based on the user's data in their network (ads are somewhat relevant to your 
browsing)

## Lecture 3
