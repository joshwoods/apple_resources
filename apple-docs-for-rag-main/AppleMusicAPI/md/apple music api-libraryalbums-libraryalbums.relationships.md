

- Apple Music API
- LibraryAlbums
-  LibraryAlbums.Relationships 

Object

# LibraryAlbums.Relationships

The relationships for a library album object.

Apple Music 1.0+

``` source
object LibraryAlbums.Relationships
```

## Properties

`artists`

LibraryAlbums.Relationships.LibraryAlbumsArtistsRelationship

The library artists associated with the album. By default, `artists` not included.

Fetch limits: 10 default, 10 maximum

`catalog`

LibraryAlbums.Relationships.LibraryAlbumsCatalogRelationship

The album in the Apple Music catalog the library album is associated with, when known.

Fetch limits: None (associated with at most one catalog album)

`tracks`

LibraryAlbums.Relationships.LibraryAlbumsTracksRelationship

The library songs and library music videos on the album. Only available when fetching single library album resource by ID. By default, `tracks` includes objects.

Fetch limits: 300 default, 300 maximum.

## Topics

### Related Objects

object LibraryAlbums.Relationships.LibraryAlbumsArtistsRelationship

A relationship from the library album to its artist.

object LibraryAlbums.Relationships.LibraryAlbumsCatalogRelationship

A relationship from the library album to its associated catalog content.

object LibraryAlbums.Relationships.LibraryAlbumsTracksRelationship

A relationship from the library album to its tracks.

## See Also

### Related Objects

object LibraryAlbums.Attributes

The attributes for a library album resource.

