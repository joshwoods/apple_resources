

- CKTool JS
- CKDBRecordsResponse
-  continuationToken 

Instance Property

# continuationToken

A string that indicates there are more records to fetch.

CKTool JS 1.2.15+

``` source
attribute string? continuationToken;
```

## Discussion

To fetch the other records, pass the value of the `continuationToken` key as the value of the `continuationToken` key in the next request.

