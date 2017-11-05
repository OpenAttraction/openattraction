# Welcome to OpenAttraction

OpenAttraction (OA) is an open-source API and database for tourist attractions. Citizens, governments and institutions are able to use OA to retrieve and store information about sites interesting for tourists in their area and use the data to build context-aware products around tourism, regional marketing and more.

This document explains the concepts, tools and methods behind the OpenAttraction.

## Database

Lacalities, places and events may be stored in a cloud database. We are using the graph database [neo4j][3], which is capable of storing information about entities and their relations between each other. Entities may be localities, places of interest, institutions, events and recommendations.

Each locality has a geo location (latitude and longitude). Places within the locality (like a museum inside a castle) are related to it. Events and other information are stored around these places and localities.

The relational character of the data, along with the geo spatial information, makes it easy to traverse and use for map-like applications.

## Tools

All information about tourist destinations is kept and presented in a human and machine readable way. We are using the [json-ld][1] protocol and [schema.org][2] topology to achieve that.

## API

All data stored in the database is accessible via HTTP interface through an API. The API is the way developers interact with the data. This way, it's possible to read the stored data, as well as add new data entities and relations and thus help to extend and grow the database and make it smarter all the time.

For instance, organizations and tourist boards are able to build marketing tools using the data, citizens may become scouts of their local area and site owners promote their loaction and events. Tourists visiting the places may comment, like and share their experiences with the world.

# Organization

t.b.d.

# Contributing

We are happy about any contribution. Please check out the document [How to contribute](HOW-TO-CONTRIBUTE.md) to learn how you can contribute.

[1]: https://json-ld.org
[2]: http://schema.org/
[3]: https://neo4j.com/product/
