

- Apple Music API
- LibraryPlaylists
-  LibraryPlaylists.Relationships 

Object

# LibraryPlaylists.Relationships

The relationships for a library playlist resource.

Apple Music 1.0+

``` source
object LibraryPlaylists.Relationships
```

## Properties

`catalog`

LibraryPlaylists.Relationships.LibraryPlaylistsCatalogRelationship

The corresponding playlist in the Apple Music catalog the playlist is associated with.

Fetch limits: None (associated with at most one catalog playlist).

`tracks`

LibraryPlaylists.Relationships.LibraryPlaylistsTracksRelationship

The library songs and library music videos included in the playlist. By default, `tracks` not included. Only available when fetching a single library playlist resource by ID.

Fetch limits: 100 default, 100 maximum.

## Topics

### Related Objects

object LibraryPlaylists.Relationships.LibraryPlaylistsCatalogRelationship

A relationship from the playlist to its associated catalog content.

object LibraryPlaylists.Relationships.LibraryPlaylistsTracksRelationship

A relationship from the playlist to its tracks.

## See Also

### Related Objects

object LibraryPlaylists.Attributes

The attributes for a library playlist resource.

