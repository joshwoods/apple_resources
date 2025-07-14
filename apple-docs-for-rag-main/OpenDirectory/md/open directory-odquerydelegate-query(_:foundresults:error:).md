

- Open Directory
- ODQueryDelegate
-  query(\_:foundResults:error:) 

Instance Method

# query(\_:foundResults:error:)

The delegate method called as results are returned from a query scheduled in a run loop.

Mac CatalystmacOS 10.6+

``` source
func query(
    _ inQuery: ODQuery!,
    foundResults inResults: [Any]!,
    error inError: (any Error)!
)
```

**Required**

## Parameters 

`inQuery`  

The query.

`inResults`  

Partial results returned from the query.

`inError`  

An error reference for error details.

## Discussion

This method is called as soon as any results become available. Results must be retained or copied. If both `inResults` and `inError` are `nil`, the query has completed.

