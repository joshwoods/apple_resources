

- Apple Music API
- LibrarySearchResponse
- LibrarySearchResponse.Results
-  LibrarySearchResponse.Results.LibraryMusicVideosSearchResult 

Object

# LibrarySearchResponse.Results.LibraryMusicVideosSearchResult

The library music videos results for a term search for specific resource types.

Apple Music 1.0+

``` source
object LibrarySearchResponse.Results.LibraryMusicVideosSearchResult
```

## Properties

`data`

`[`LibraryMusicVideos`]`

 (Required) 

The library music video resources matching the search term, ordered by best match.

`href`

`string`

A relative location for the resource.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources if more exist.

## See Also

### Related Objects

object LibrarySearchResponse.Results.LibraryAlbumsSearchResult

The library albums results for a term search for specific resource types.

object LibrarySearchResponse.Results.LibraryArtistsSearchResult

The library artists results for a term search for specific resource types.

object LibrarySearchResponse.Results.LibraryPlaylistsSearchResult

The library playlists results for a term search for specific resource types.

object LibrarySearchResponse.Results.LibrarySongsSearchResult

The library songs results for a term search for specific resource types.

