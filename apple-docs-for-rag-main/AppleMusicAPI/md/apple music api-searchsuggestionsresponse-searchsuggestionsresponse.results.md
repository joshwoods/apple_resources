

- Apple Music API
- SearchSuggestionsResponse
-  SearchSuggestionsResponse.Results 

Object

# SearchSuggestionsResponse.Results

An object that represents the results of a search suggestions query.

Apple Music 1.0+

``` source
object SearchSuggestionsResponse.Results
```

## Properties

`suggestions`

`[*]`

 (Required) 

An array of possible valid search queries determined from the search suggestion.

Possible types: SearchSuggestionsResponse.Results.TermSuggestion`, `SearchSuggestionsResponse.Results.TopResultSuggestion

## Topics

### Related Objects

object SearchSuggestionsResponse.Results.TermSuggestion

A suggested search term from a search suggestion response.

object SearchSuggestionsResponse.Results.TopResultSuggestion

A suggested popular result for similar search prefix terms.

