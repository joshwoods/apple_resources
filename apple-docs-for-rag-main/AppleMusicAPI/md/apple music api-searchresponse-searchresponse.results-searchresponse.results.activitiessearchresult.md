

- Apple Music API
- SearchResponse
- SearchResponse.Results
-  SearchResponse.Results.ActivitiesSearchResult 

Object

# SearchResponse.Results.ActivitiesSearchResult

An object containing an activities’ search result.

Apple Music 1.0+

``` source
object SearchResponse.Results.ActivitiesSearchResult
```

## Properties

`data`

`[`Activities`]`

 (Required) 

The resources for the search result.

`href`

`string`

The relative location to fetch the search result.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the result, if more exist.

## See Also

### Related Objects

object SearchResponse.Results.AlbumsSearchResult

An object containing an albums’ search result.

object SearchResponse.Results.AppleCuratorsSearchResult

An object containing the Apple curators’ search result.

object SearchResponse.Results.ArtistsSearchResult

An object containing an artists’ search result.

object SearchResponse.Results.CuratorsSearchResult

An object containing a curators’ search result.

object SearchResponse.Results.MusicVideosSearchResult

An object containing a music videos’ search result.

object SearchResponse.Results.PlaylistsSearchResult

An object containing a playlists’ search result.

object SearchResponse.Results.RecordLabelsSearchResult

An object containing a record labels’ search result.

object SearchResponse.Results.SongsSearchResult

An object containing a songs’ search result.

object SearchResponse.Results.StationsSearchResult

An object containing a stations’ search result.

object SearchResponse.Results.TopResultsSearchResult

An object containing a top results’ search result.

