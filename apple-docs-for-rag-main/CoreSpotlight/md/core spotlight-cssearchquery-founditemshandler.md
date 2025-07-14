

- Core Spotlight
- CSSearchQuery
-  foundItemsHandler 

Instance Property

# foundItemsHandler

The block to execute when the query delivers a new batch of matching items.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
var foundItemsHandler: (([CSSearchableItem]) -> Void)? { get set }
```

## Mentioned in 

Searching for information in your app

Building a search interface for your app

## Discussion

Assign a block to this property that has no return value and takes the following parameter:

items  
An array of items that match the specified query.

Specify a value for this property only if you start your query with the start() method. While the query runs, the query object executes the provided closure one or more times to deliver suggested search results for the current search term. Use your handler to retrieve the those results and display them. The query object stops delivering matching items when it reaches the maximum number found in the maxResultCount property of the query configuration parameters.

Each time the query object calls your handler, it delivers only the new items that it found since the last time it called your handler. However, the query object updates the value of the foundItemCount property with the total number of items before it calls your handler.

If you start the query by accessing the results property of CSSearchQuery or the responses property of CSUserQuery, the query object doesn’t execute the block in this property. property of CSUserQuery, the query object doesn’t execute the block in this property.

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

var completionHandler: (((any Error)?) -> Void)?

The block to execute when the query finishes delivering all results.

