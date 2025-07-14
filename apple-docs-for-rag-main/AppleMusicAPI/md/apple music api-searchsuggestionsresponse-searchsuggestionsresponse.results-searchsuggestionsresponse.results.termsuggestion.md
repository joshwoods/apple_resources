

- Apple Music API
- SearchSuggestionsResponse
- SearchSuggestionsResponse.Results
-  SearchSuggestionsResponse.Results.TermSuggestion 

Object

# SearchSuggestionsResponse.Results.TermSuggestion

A suggested search term from a search suggestion response.

Apple Music 1.0+

``` source
object SearchSuggestionsResponse.Results.TermSuggestion
```

## Properties

`displayTerm`

`string`

 (Required) 

A potentially censored term to display to the user to select from. Use the `searchTerm` value for the actual search.

`kind`

`string`

 (Required) 

The kind of suggestion.

Value: `terms`

`searchTerm`

`string`

 (Required) 

The term to use as a search input when using this suggestion.

## See Also

### Related Objects

object SearchSuggestionsResponse.Results.TopResultSuggestion

A suggested popular result for similar search prefix terms.

