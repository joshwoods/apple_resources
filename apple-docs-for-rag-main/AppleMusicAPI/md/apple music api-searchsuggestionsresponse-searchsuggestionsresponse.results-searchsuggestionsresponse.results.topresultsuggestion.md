

- Apple Music API
- SearchSuggestionsResponse
- SearchSuggestionsResponse.Results
-  SearchSuggestionsResponse.Results.TopResultSuggestion 

Object

# SearchSuggestionsResponse.Results.TopResultSuggestion

A suggested popular result for similar search prefix terms.

Apple Music 1.0+

``` source
object SearchSuggestionsResponse.Results.TopResultSuggestion
```

## Properties

`content`

`(`Activities` | `Albums` | `AppleCurators` | `Artists` | `Curators` | `MusicVideos` | `Playlists` | `RecordLabels` | `Songs` | `Stations`)`

 (Required) 

The actual resource for the suggested content.

Possible types: Activities`, `Albums`, `AppleCurators`, `Artists`, `Curators`, `MusicVideos`, `Playlists`, `RecordLabels`, `Songs`, `Stations

`kind`

`string`

 (Required) 

The kind of suggestion.

Value: `topResults`

## See Also

### Related Objects

object SearchSuggestionsResponse.Results.TermSuggestion

A suggested search term from a search suggestion response.

