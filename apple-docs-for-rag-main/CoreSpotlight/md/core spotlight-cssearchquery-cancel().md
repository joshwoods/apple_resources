

- Core Spotlight
- CSSearchQuery
-  cancel() 

Instance Method

# cancel()

Cancels the current query operation.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func cancel()
```

## Mentioned in 

Searching for information in your app

## Discussion

Cancel a query operation when you no longer need the results. You can use this method to cancel a query you started, by using either the start() method or by accessing the results property. After you cancel a query operation, you can’t restart it. To perform a new query, create a new query object. For example, you might cancel one query and start a new one when the text in your app’s search control changes.

## See Also

### Executing the query with handler blocks

func start()

Starts searching the index for items that match the current query string and parameters.

var isCancelled: Bool

A Boolean value that indicates whether the current query is no longer running.

var foundItemCount: Int

The number of matching items found for the given query string.

var foundItemsHandler: (([CSSearchableItem]) -> Void)?

The block to execute when the query delivers a new batch of matching items.

var completionHandler: (((any Error)?) -> Void)?

The block to execute when the query finishes delivering all results.

