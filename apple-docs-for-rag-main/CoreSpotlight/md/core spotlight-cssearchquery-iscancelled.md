

- Core Spotlight
- CSSearchQuery
-  isCancelled 

Instance Property

# isCancelled

A Boolean value that indicates whether the current query is no longer running.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
var isCancelled: Bool { get }
```

## Discussion

The value of this property is `true` if you canceled it, and `false` if it’s still running or able to run.

## See Also

### Executing the query with handler blocks

func start()

Starts searching the index for items that match the current query string and parameters.

func cancel()

Cancels the current query operation.

var foundItemCount: Int

The number of matching items found for the given query string.

var foundItemsHandler: (([CSSearchableItem]) -> Void)?

The block to execute when the query delivers a new batch of matching items.

var completionHandler: (((any Error)?) -> Void)?

The block to execute when the query finishes delivering all results.

