

- Core Spotlight
- CSUserQueryContext
-  maxSuggestionCount 

Instance Property

# maxSuggestionCount

The maximum number of suggested text completions for the query to return.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var maxSuggestionCount: Int { get set }
```

## Discussion

You might specify different limits to account for the amount of available space.

## See Also

### Configuring search options

var maxResultCount: Int

The maximum number of search results for the query to return.

var disableSemanticSearch: Bool

A Boolean value that indicates whether to exclude semantic-based search results from the output.

