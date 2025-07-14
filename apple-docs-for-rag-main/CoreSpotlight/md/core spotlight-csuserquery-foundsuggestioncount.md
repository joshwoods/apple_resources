

- Core Spotlight
- CSUserQuery
-  foundSuggestionCount 

Instance Property

# foundSuggestionCount

The number of suggested items the query found so far.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var foundSuggestionCount: Int { get }
```

## Discussion

As the query runs, it updates the value in this property to reflect the total number of suggestions.

## See Also

### Executing the query with handler blocks

func start()

Starts searching the index for items that match the current query string and parameters.

func cancel()

Cancels the current query operation.

var foundSuggestionsHandler: (([CSSuggestion]) -> Void)?

The block to execute when the query delivers a new batch of suggested items.

