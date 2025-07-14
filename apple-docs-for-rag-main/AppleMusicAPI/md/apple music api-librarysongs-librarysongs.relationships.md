

- Apple Music API
- LibrarySongs
-  LibrarySongs.Relationships 

Object

# LibrarySongs.Relationships

The relationships for a library song resource.

Apple Music 1.0+

``` source
object LibrarySongs.Relationships
```

## Properties

`albums`

LibrarySongs.Relationships.LibrarySongsAlbumsRelationship

The library albums associated with the song. By default, `albums` not included.

Fetch limits: 10 default, 10 maximum.

`artists`

LibrarySongs.Relationships.LibrarySongsArtistsRelationship

The library artists associated with the song. By default, `artists` not included.

Fetch limits: 10 default, 10 maximum.

`catalog`

LibrarySongs.Relationships.LibrarySongsCatalogRelationship

The song in the Apple Music catalog the library song is associated with, when known.

Fetch limits: None.

## Topics

### Related Objects

object LibrarySongs.Relationships.LibrarySongsAlbumsRelationship

A relationship from the library song to its albums.

object LibrarySongs.Relationships.LibrarySongsArtistsRelationship

A relationship from the library song to its artists.

object LibrarySongs.Relationships.LibrarySongsCatalogRelationship

A relationship from the library song to its associated catalog content.

## See Also

### Related Objects

object LibrarySongs.Attributes

The attributes for a library song resource.

