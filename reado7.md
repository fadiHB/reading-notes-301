# REPRESENTATIONAL STATE TRANSFER

REST, or REpresentational State Transfer, is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other. REST-compliant systems, often called RESTful systems, are characterized by how they are stateless and separate the concerns of client and server. We will go into what these terms mean and why they are beneficial characteristics for services on the Web.

## MAKING REQUESTS
REST requires that a client make a request to the server in order to retrieve or modify data on the server. A request generally consists of:

an HTTP verb, which defines what kind of operation to perform
a header, which allows the client to pass along information about the request
a path to a resource
an optional message body containing data
HTTP VERBS
There are 4 basic HTTP verbs we use in requests to interact with resources in a REST system:

1. GET — retrieve a specific resource (by id) or a collection of resources
2. POST — create a new resource
3. PUT — update a specific resource (by id)
4. DELETE — remove a specific resource by id

## SuperAgent

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!