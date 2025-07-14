

- Media Player
-  MPMediaItemPropertyAssetURL 

Global Variable

# MPMediaItemPropertyAssetURL

A URL that points to the media item.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
let MPMediaItemPropertyAssetURL: String
```

## Discussion

This value is an NSURL object. The URL has the custom scheme of `ipod-library`. For example, a URL might look like this:

- Swift
- Objective-C

```
ipod-library://item/item.m4a?id=12345
```

```
ipod-library://item/item.m4a?id=12345
```

## See Also

### Property keys

let MPMediaItemPropertyPlaybackDuration: String

The playback duration of the media item.

let MPMediaItemPropertyAlbumTrackNumber: String

The track number of the media item, for a media item that is part of an album.

let MPMediaItemPropertyAlbumTrackCount: String

The number of tracks for the album that contains the media item.

let MPMediaItemPropertyDiscNumber: String

The disc number of the media item, for a media item that is part of a multidisc album.

let MPMediaItemPropertyDiscCount: String

The number of discs for the album that contains the media item.

let MPMediaItemPropertyArtwork: String

The artwork image for the media item.

let MPMediaItemPropertyLyrics: String

The lyrics for the media item.

let MPMediaItemPropertyReleaseDate: String

The date of the media item’s first public release.

let MPMediaItemPropertyBeatsPerMinute: String

The number of musical beats per minute for the media item.

let MPMediaItemPropertyComments: String

Textual information about the media item.

let MPMediaItemPropertyIsExplicit: String

A Boolean value that indicates whether the media item contains explicit (adult) lyrics or language.

let MPMediaItemPropertyIsPreorder: String

A Boolean value that indicates whether the media item is a preorder.

let MPMediaItemPropertyPlaybackStoreID: String

The identifier for enqueueing store tracks.

