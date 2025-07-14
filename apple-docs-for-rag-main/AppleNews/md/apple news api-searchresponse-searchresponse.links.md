

- Apple News API
- SearchResponse
-  SearchResponse.Links 

Object

# SearchResponse.Links

See the links the search article endpoints returned.

Apple News API 1.0+

``` source
object SearchResponse.Links
```

## Properties

`self`

`string`

The URL for the current page of search results.

`next`

`string`

The URL for the next page of search results. If `next` is null, there are no more pages. The `next` link may occasionally return an empty page of results.

