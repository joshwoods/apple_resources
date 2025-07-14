

- Core Spotlight
- CSUserQuery
-  foundSuggestionsHandler 

Instance Property

# foundSuggestionsHandler

The block to execute when the query delivers a new batch of suggested items.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var foundSuggestionsHandler: (([CSSuggestion]) -> Void)? { get set }
```

## Mentioned in 

Building a search interface for your app

## Discussion

Specify a value for this property only if you start your query with the start() method. While the query runs, the query object executes the provided closure one or more times to deliver suggested completions for the current search term. Use your handler to retrieve the suggested completions and update your app’s search interface. The query object stops delivering suggested items when it runs out of suggestions or reaches the maximum number found in the maxSuggestionCount property of the query configuration parameters.

If you start the query by accessing the responses property, the query object doesn’t execute the block in this property.

## See Also

### Executing the query with handler blocks

func start()

Starts searching the index for items that match the current query string and parameters.

func cancel()

Cancels the current query operation.

var foundSuggestionCount: Int

The number of suggested items the query found so far.

