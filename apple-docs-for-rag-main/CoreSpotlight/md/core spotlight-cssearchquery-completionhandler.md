

- Core Spotlight
- CSSearchQuery
-  completionHandler 

Instance Property

# completionHandler

The block to execute when the query finishes delivering all results.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
var completionHandler: (((any Error)?) -> Void)? { get set }
```

## Mentioned in 

Searching for information in your app

## Discussion

Specify a value for this property only if you start your query with the start() method. When the query finishes, the query object executes the provided closure once to let you know the search is complete. Use your handler to perform any related cleanup. The block you assign to this property returns no parameters and takes the following parameter:

error  
An error object with details about a problem that occurred, or `nil` if the query completed successfully.

If you start the query by accessing the results property of CSSearchQuery or the responses property of CSUserQuery, the query object doesn’t execute the block in this property.

## See Also

### Executing the query with handler blocks

func start()

Starts searching the index for items that match the current query string and parameters.

func cancel()

Cancels the current query operation.

var isCancelled: Bool

A Boolean value that indicates whether the current query is no longer running.

var foundItemCount: Int

The number of matching items found for the given query string.

var foundItemsHandler: (([CSSearchableItem]) -> Void)?

The block to execute when the query delivers a new batch of matching items.

