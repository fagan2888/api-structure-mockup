## The framework
The API framework is organized into two main access points: Search and Access. The Search access point is used to retrieve content metadata about tables, maps, data, and webpages. The content metadata responses all include access urls which may be used to access the underlying content (table, data, map, or webpage).

Here is a quick overview of the basic structure:
```
api.census.gov
│   README.md
│   endpoints
│
└───search
|   │   endpoints
│   │   quickAnswer
│   │   tables
│   │   maps
│   │   pages
│   
└───access
|   │   endpoints
│   │   quickAnswer
│   │   tables
│   │   maps
│   │   pages
```

The objective with this structure is to organize the access points by user intent (/search for searching through metadata or /access for accessing data), and then provide pathways that allow users to further specify by content type (tables, maps, webpages, or quickanswers).

## Parameters
The method to specify content is used through global and local parameters. Global parameters may be used for any endpoint and are consistent while local parameters are specific to each endpoint.

With global parameters, users can execute valid requests against /search, /access, or any pathway using the same parameter set. The response objects will vary
