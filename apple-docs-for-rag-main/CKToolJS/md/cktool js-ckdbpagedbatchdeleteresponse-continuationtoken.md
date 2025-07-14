

- CKTool JS
- CKDBPagedBatchDeleteResponse
-  continuationToken 

Instance Property

# continuationToken

A string value that indicates there are more results to fetch.

CKTool JS 1.2.15+

``` source
attribute string? continuationToken;
```

## Discussion

To fetch the other results, pass the value of the continuationToken key as the value of the continuationToken key in the next request.

