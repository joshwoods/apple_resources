

- Foundation
- NSMetadataQuery
-  isStopped 

Instance Property

# isStopped

A Boolean value that indicates whether the query has stopped.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isStopped: Bool { get }
```

## Discussion

This property contains true when the receiver has stopped the query; otherwise, false.

## See Also

### Running Queries

var isStarted: Bool

A Boolean value that indicates whether the query has started. (read-only)

func start() -> Bool

Attempts to start the query.

var isGathering: Bool

A Boolean value that indicates whether the receiver is in the initial gathering phase of the query. (read-only)

func stop()

Stops the receiver’s current query from gathering any further results.

