

- Apple Music API
- LibraryPlaylistCreationRequest
- LibraryPlaylistCreationRequest.Relationships
-  LibraryPlaylistCreationRequest.Relationships.Tracks 

Object

# LibraryPlaylistCreationRequest.Relationships.Tracks

The songs and music videos to add to the created playlist’s tracklist.

Apple Music 1.0+

``` source
object LibraryPlaylistCreationRequest.Relationships.Tracks
```

## Properties

`data`

`[`LibraryPlaylistCreationRequest.Relationships.Tracks.Data`]`

 (Required) 

A dictionary that includes strings for the `identifier` and `type` of the new playlist.

## Topics

### Related Objects

object LibraryPlaylistCreationRequest.Relationships.Tracks.Data

Data of the tracks too add to the created library playlist.

## See Also

### Related Objects

object LibraryPlaylistCreationRequest.Relationships.Parent

Library playlist folder which contains the playlist that the user creates.

