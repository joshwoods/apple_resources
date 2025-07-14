

- Core Spotlight
- CSUserQueryContext
-  maxResultCount 

Instance Property

# maxResultCount

The maximum number of search results for the query to return.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var maxResultCount: Int { get set }
```

## Discussion

Spotlight returns all results that it finds by default. Set a maximum limit to terminate the search early, which can improve performance.

## See Also

### Configuring search options

var maxSuggestionCount: Int

The maximum number of suggested text completions for the query to return.

var disableSemanticSearch: Bool

A Boolean value that indicates whether to exclude semantic-based search results from the output.

