

- Apple Music API
- LibraryMusicVideos
- LibraryMusicVideos.Relationships
-  LibraryMusicVideos.Relationships.LibraryMusicVideosArtistsRelationship 

Object

# LibraryMusicVideos.Relationships.LibraryMusicVideosArtistsRelationship

A relationship from the library music video to its artists in the library.

Apple Music 1.0+

``` source
object LibraryMusicVideos.Relationships.LibraryMusicVideosArtistsRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`LibraryArtists`]`

 (Required) 

The artists in the library the music video is associated with.

## See Also

### Related Objects

object LibraryMusicVideos.Relationships.LibraryMusicVideosAlbumsRelationship

A relationship from the library music video to its albums in the library.

object LibraryMusicVideos.Relationships.LibraryMusicVideosCatalogRelationship

A relationship from the library music video to its associated catalog content.

