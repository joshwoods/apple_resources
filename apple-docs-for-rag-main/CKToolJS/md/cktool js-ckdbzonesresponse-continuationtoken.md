

- CKTool JS
- CKDBZonesResponse
-  continuationToken 

Instance Property

# continuationToken

A string value that indicates that there are more zones to fetch.

CKTool JS 1.2.15+

``` source
attribute string? continuationToken;
```

## Discussion

To fetch the other zones, pass the value of `continuationToken` as the `continuationToken` value in the next request

