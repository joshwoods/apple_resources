

- Core Spotlight
- CSSearchQuery
-  foundItemCount 

Instance Property

# foundItemCount

The number of matching items found for the given query string.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
var foundItemCount: Int { get }
```

## Discussion

As Spotlight finds matches to the query string, it updates the value of this property and delivers the new results to the handler in the foundItemsHandler property. This value reflects the total number of matching items, including the number of items the query delivered to your handler block previously.

## See Also

### Executing the query with handler blocks

func start()

Starts searching the index for items that match the current query string and parameters.

func cancel()

Cancels the current query operation.

var isCancelled: Bool

A Boolean value that indicates whether the current query is no longer running.

var foundItemsHandler: (([CSSearchableItem]) -> Void)?

The block to execute when the query delivers a new batch of matching items.

var completionHandler: (((any Error)?) -> Void)?

The block to execute when the query finishes delivering all results.

