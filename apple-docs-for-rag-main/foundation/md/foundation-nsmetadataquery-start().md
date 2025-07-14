

- Foundation
- NSMetadataQuery
-  start() 

Instance Method

# start()

Attempts to start the query.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func start() -> Bool
```

## Return Value

true when successful; otherwise, false.

A query may fail to start if it does not specify a predicate, or if the query has already been started.

## Discussion

A query can’t be started if the receiver is already running a query or no predicate has been specified.

This method must be called from the receiver’s operationQueue or on the main thread. For example:

- Swift
- Objective-C

```
let query: NSMetadataQuery = // Initialize and set up a query
    query.operationQueue?.addOperationWithBlock {
        query.startQuery()
}
```

```
NSMetadataQuery *query = // Initialize and set up a query
[query.operationQueue addOperationWithBlock:^{
    [query startQuery];
}];
```

## See Also

### Running Queries

var isStarted: Bool

A Boolean value that indicates whether the query has started. (read-only)

var isGathering: Bool

A Boolean value that indicates whether the receiver is in the initial gathering phase of the query. (read-only)

var isStopped: Bool

A Boolean value that indicates whether the query has stopped.

func stop()

Stops the receiver’s current query from gathering any further results.

