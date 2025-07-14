

- Core Spotlight
- CSUserQuery
-  start() 

Instance Method

# start()

Starts searching the index for items that match the current query string and parameters.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func start()
```

## Mentioned in 

Building a search interface for your app

## Discussion

This method uses the configured search parameters and query string to begin a search of the index. It then delivers the results of that search to the closures in the foundItemsHandler, foundSuggestionsHandler, and completionHandler properties of the query object.

Note

Don’t call this method if you fetch the query results using the responses property. Accessing that property automatically starts the query.

## See Also

### Executing the query with handler blocks

func cancel()

Cancels the current query operation.

var foundSuggestionsHandler: (([CSSuggestion]) -> Void)?

The block to execute when the query delivers a new batch of suggested items.

var foundSuggestionCount: Int

The number of suggested items the query found so far.

