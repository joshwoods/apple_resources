

- MusicKit
- MusicLibrary
-  createPlaylist(name:description:authorDisplayName:items:) 

Instance Method

# createPlaylist(name:description:authorDisplayName:items:)

Creates a playlist in the user’s music library.

iOS 16.0+iPadOS 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@discardableResult
func createPlaylist(
    name: String,
    description: String? = nil,
    authorDisplayName: String? = nil,
    items: S
) async throws -> Playlist where S : Sequence, MusicPlaylistAddableType : MusicPlaylistAddable, MusicPlaylistAddableType == S.Element
```

## Parameters 

`name`  

The name of the playlist.

`description`  

An optional description of the playlist.

`authorDisplayName`  

The display name of the author for the playlist. A `nil` value will result in the framework using your app’s name instead.

`items`  

The items of the playlist.

## Return Value

The newly created playlist.

