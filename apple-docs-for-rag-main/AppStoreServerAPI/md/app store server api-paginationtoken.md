

- App Store Server API
-  paginationToken 

Type

# paginationToken

A pagination token that you return to the endpoint on a subsequent call to receive the next set of results.

App Store Server API 1.5+

``` source
string paginationToken
```

## Discussion

A token you use in the Get Notification History endpoint to ask for the next set of up to 20 notification history entries. All responses include a `paginationToken`.

## See Also

### Data types

type hasMore

A Boolean value indicating whether the App Store has more transaction data.

