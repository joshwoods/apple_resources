

- Media Player
- MPContentItem
-  isPlayable 

Instance Property

# isPlayable

A Boolean value that indicates whether a media item is able to be played.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+

``` source
var isPlayable: Bool { get set }
```

## Discussion

When set to true, the designated content item is able to be played. Containers and individual content items can set this property to true. For example, a playlist with multiple songs in it. The playlist is a container that can be played, or the user could choose a song from inside of the playlist.

## See Also

### Retrieving information about a media item

var artwork: MPMediaItemArtwork?

A single image that’s associated with the media item.

var isContainer: Bool

A Boolean value that indicates whether a media item is container of other items.

var isExplicitContent: Bool

A Boolean value that indicates whether the media item contains explicit content.

var identifier: String

The unique identifier for the media item.

var isStreamingContent: Bool

A Boolean value that indicates whether the content item is streaming content.

var playbackProgress: Float

The amount of content played for the media item.

var subtitle: String?

A secondary designator for the media item.

var title: String?

The public name of the media item.

