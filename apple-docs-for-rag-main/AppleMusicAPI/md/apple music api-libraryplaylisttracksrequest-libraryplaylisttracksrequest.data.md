

- Apple Music API
- LibraryPlaylistTracksRequest
-  LibraryPlaylistTracksRequest.Data 

Object

# LibraryPlaylistTracksRequest.Data

An object that represents a single track when added to a library playlist in a request.

Apple Music 1.0+

``` source
object LibraryPlaylistTracksRequest.Data
```

## Properties

`id`

`string`

 (Required) 

The unique identifier of the library playlist track.

`type`

`string`

 (Required) 

The type of the track to be added. The possible values are `library-music-videos`, `library-songs`, `music-videos`, or `songs`.

Possible Values: `library-music-videos, library-songs, music-videos, songs`

