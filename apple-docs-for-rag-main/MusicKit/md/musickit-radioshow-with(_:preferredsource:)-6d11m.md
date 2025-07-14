

- MusicKit
- RadioShow
-  with(\_:preferredSource:) 

Instance Method

# with(\_:preferredSource:)

Loads a new instance of the music item that includes the specified properties.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func with(
    _ properties: PartialMusicAsyncProperty...,
    preferredSource: MusicPropertySource
) async throws -> Self
```

Available when `Self` conforms to `MusicPropertyContainer` and `Decodable`.

## Discussion

This asynchronous method fetches a more complete representation of the receiver, loading the contents for each property you request from either the Apple Music catalog or the user’s library, depending on the preferred source as well the availability of the content in those respective data sources.

For example, if you want to load the tracks relationship for an Album, as found in the user’s library, as well as other associations of content that only live in the Apple Music catalog, like the recordLabels and relatedAlbums associations, you can use this code:

```
let album: Album = …
let detailedAlbum = try await album.with(
    .tracks,
    .recordLabels,
    .relatedAlbums, 
    preferredSource: .library
)
```

Here, because the tracks relationship for an Album is supported in both the library and the catalog, and because the this code specifically requests MusicPropertySource.library as the preferred source, the framework will load the tracks from the user’s library. However, because the recordLabels and relatedAlbums associations are only available in the Apple Music catalog, the framework will also issue a network request to Apple Music API to fetch those associations of content from the catalog.

