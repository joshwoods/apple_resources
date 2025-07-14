

- Apple Music API
- Albums
- Albums.Relationships
-  Albums.Relationships.AlbumsTracksRelationship 

Object

# Albums.Relationships.AlbumsTracksRelationship

A relationship from the album to its tracks.

Apple Music 1.0+

``` source
object Albums.Relationships.AlbumsTracksRelationship
```

## Properties

`data`

`[*]`

 (Required) 

The ordered songs and music videos in the tracklist of the album.

Possible types: MusicVideos`, `Songs

`href`

`string`

A relative location for the relationship.

`next`

`string`

A relative cursor to fetch the next paginated collection of resources in the relationship if more exist.

## See Also

### Related Objects

object Albums.Relationships.AlbumsArtistsRelationship

A relationship from the album to its artists.

object Albums.Relationships.AlbumsGenresRelationship

A relationship from the album to its genres.

object Albums.Relationships.AlbumsLibraryRelationship

A relationship from the album to an associated library album.

object Albums.Relationships.AlbumsRecordLabelsRelationship

A relationship from the album to its associated record label.

