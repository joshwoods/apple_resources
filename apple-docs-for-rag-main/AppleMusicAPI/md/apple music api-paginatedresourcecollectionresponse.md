

- Apple Music API
-  PaginatedResourceCollectionResponse 

Object

# PaginatedResourceCollectionResponse

A response object composed of paginated resource objects for the request.

Apple Music 1.0+

``` source
object PaginatedResourceCollectionResponse
```

## Properties

`next`

`string`

A relative cursor to fetch the next paginated collection of resources for the request if more exist.

`data`

`[`Resource`]`

 (Required) 

A paginated collection of resources for the request.

