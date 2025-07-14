

- Apple Music API
- LibraryMusicVideos
- LibraryMusicVideos.Relationships
-  LibraryMusicVideos.Relationships.LibraryMusicVideosCatalogRelationship 

Object

# LibraryMusicVideos.Relationships.LibraryMusicVideosCatalogRelationship

A relationship from the library music video to its associated catalog content.

Apple Music 1.0+

``` source
object LibraryMusicVideos.Relationships.LibraryMusicVideosCatalogRelationship
```

## Properties

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

`data`

`[`MusicVideos`]`

 (Required) 

The music video from the Apple Music catalog associated with the library music video, if any.

## See Also

### Related Objects

object LibraryMusicVideos.Relationships.LibraryMusicVideosAlbumsRelationship

A relationship from the library music video to its albums in the library.

object LibraryMusicVideos.Relationships.LibraryMusicVideosArtistsRelationship

A relationship from the library music video to its artists in the library.

