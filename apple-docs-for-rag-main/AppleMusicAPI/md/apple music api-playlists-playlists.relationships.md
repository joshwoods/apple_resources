

- Apple Music API
- Playlists
-  Playlists.Relationships 

Object

# Playlists.Relationships

The relationships for a playlist resource.

Apple Music 1.0+

``` source
object Playlists.Relationships
```

## Properties

`curator`

Playlists.Relationships.PlaylistsCuratorRelationship

The curator that created the playlist. By default, `curator` includes identifiers only.

Fetch limits: None

`library`

Playlists.Relationships.PlaylistsLibraryRelationship

Library playlist for a catalog playlist if added to library.

`tracks`

Playlists.Relationships.PlaylistsTracksRelationship

The songs and music videos included in the playlist. By default, `tracks` includes objects.

Fetch limits: 100 default, 300 maximum

## Topics

### Related Objects

object Playlists.Relationships.PlaylistsCuratorRelationship

A relationship from the playlist to its curator.

object Playlists.Relationships.PlaylistsTracksRelationship

A relationship from the playlist to its tracks.

object Playlists.Relationships.PlaylistsLibraryRelationship

A relationship from the playlist to its library.

## See Also

### Related Objects

object Playlists.Attributes

The attributes for a playlist resource.

object Playlists.Views

The views for a music video resource.

