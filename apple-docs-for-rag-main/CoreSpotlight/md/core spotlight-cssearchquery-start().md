

- Core Spotlight
- CSSearchQuery
-  start() 

Instance Method

# start()

Starts searching the index for items that match the current query string and parameters.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func start()
```

## Mentioned in 

Searching for information in your app

## Discussion

This method uses the configured search parameters and query string to begin a search of the index. It then delivers the results of that search to the closures in the foundItemsHandler and completionHandler properties of the query object.

Note

Don’t call this method if you fetch the query results using the results property. Accessing that property automatically starts the query.

## See Also

### Executing the query with handler blocks

func cancel()

Cancels the current query operation.

var isCancelled: Bool

A Boolean value that indicates whether the current query is no longer running.

var foundItemCount: Int

The number of matching items found for the given query string.

var foundItemsHandler: (([CSSearchableItem]) -> Void)?

The block to execute when the query delivers a new batch of matching items.

var completionHandler: (((any Error)?) -> Void)?

The block to execute when the query finishes delivering all results.

