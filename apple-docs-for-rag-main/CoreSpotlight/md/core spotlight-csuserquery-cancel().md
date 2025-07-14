

- Core Spotlight
- CSUserQuery
-  cancel() 

Instance Method

# cancel()

Cancels the current query operation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
func cancel()
```

## Discussion

Cancel a query operation when you no longer need the results. You can use this method to cancel queries started using either the start() method or by accessing the responses property. After you cancel a query operation, you can’t restart it. To perform a new query, create a new query object. For example, you might cancel one query and start a new one when the text in your app’s search control changes.

## See Also

### Executing the query with handler blocks

func start()

Starts searching the index for items that match the current query string and parameters.

var foundSuggestionsHandler: (([CSSuggestion]) -> Void)?

The block to execute when the query delivers a new batch of suggested items.

var foundSuggestionCount: Int

The number of suggested items the query found so far.

