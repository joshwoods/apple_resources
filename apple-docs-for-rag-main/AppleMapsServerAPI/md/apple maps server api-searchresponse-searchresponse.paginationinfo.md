

- Apple Maps Server API
- SearchResponse
-  SearchResponse.PaginationInfo 

Object

# SearchResponse.PaginationInfo

An object that returns a page of search responses.

Apple Maps Server API 1.2+

``` source
object SearchResponse.PaginationInfo
```

## Properties

`nextPageToken`

`string`

An opaque string that the server uses to fetch the next page of search responses.

`prevPageToken`

`string`

An opaque string that the server uses to fetch the previous page of search responses.

`totalPageCount`

`number`

The total number of pages for the request.

`totalResults`

`number`

The total number of results for the request.

## See Also

### Place information returned by a search

object SearchResponse.Place

A structure returned by a search that describes a place.

