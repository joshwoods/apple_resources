

- MusicKit
- MusicLibrary
-  add(\_:to:) 

Instance Method

# add(\_:to:)

Adds an item to the end of an existing playlist.

iOS 16.0+iPadOS 16.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@discardableResult
func add(
    _ item: MusicItemType,
    to playlist: Playlist
) async throws -> Playlist where MusicItemType : MusicPlaylistAddable
```

## Return Value

The updated playlist.

