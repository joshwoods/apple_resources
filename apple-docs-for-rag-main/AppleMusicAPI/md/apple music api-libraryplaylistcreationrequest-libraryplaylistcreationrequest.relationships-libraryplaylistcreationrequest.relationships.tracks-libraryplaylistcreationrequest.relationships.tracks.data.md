

- Apple Music API
- LibraryPlaylistCreationRequest
- LibraryPlaylistCreationRequest.Relationships
- LibraryPlaylistCreationRequest.Relationships.Tracks
-  LibraryPlaylistCreationRequest.Relationships.Tracks.Data 

Object

# LibraryPlaylistCreationRequest.Relationships.Tracks.Data

Data of the tracks too add to the created library playlist.

Apple Music 1.0+

``` source
object LibraryPlaylistCreationRequest.Relationships.Tracks.Data
```

## Properties

`id`

`string`

 (Required) 

The unique identifier for the track. This ID can be a catalog identifier or a library identifier, depending on the track type.

`type`

`string`

 (Required) 

The type of the track to be added.

Possible Values: `library-music-videos, library-songs, music-videos, songs`

