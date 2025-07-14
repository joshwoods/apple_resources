

- Apple Music API
- LibraryArtists
-  LibraryArtists.Relationships 

Object

# LibraryArtists.Relationships

The relationships for a library artist resource.

Apple Music 1.0+

``` source
object LibraryArtists.Relationships
```

## Properties

`albums`

LibraryArtists.Relationships.LibraryArtistsAlbumsRelationship

The library albums associated with the artist. By default, `albums` not included. It’s available only when fetching a single library artist resource by ID.

Fetch limits: 25 default, 100 maximum

`catalog`

LibraryArtists.Relationships.LibraryArtistsCatalogRelationship

The artist in the Apple Music catalog the library artist is associated with, when known.

Fetch limits: None (associated with, at most, one catalog artist).

## Topics

### Related Objects

object LibraryArtists.Relationships.LibraryArtistsAlbumsRelationship

A relationship from the library artist to thier albums.

object LibraryArtists.Relationships.LibraryArtistsCatalogRelationship

A relationship from the library artist to their associated catalog content.

## See Also

### Related Objects

object LibraryArtists.Attributes

The attributes for a library artist resource.

