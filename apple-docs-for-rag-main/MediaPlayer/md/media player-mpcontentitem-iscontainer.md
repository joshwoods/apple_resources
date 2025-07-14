

- Media Player
- MPContentItem
-  isContainer 

Instance Property

# isContainer

A Boolean value that indicates whether a media item is container of other items.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+

``` source
var isContainer: Bool { get set }
```

## Discussion

When set to true, the designated content item’s identified as being able to contain other content items. For example, an album is a container that holds multiple songs.

## See Also

### Retrieving information about a media item

var artwork: MPMediaItemArtwork?

A single image that’s associated with the media item.

var isExplicitContent: Bool

A Boolean value that indicates whether the media item contains explicit content.

var identifier: String

The unique identifier for the media item.

var isPlayable: Bool

A Boolean value that indicates whether a media item is able to be played.

var isStreamingContent: Bool

A Boolean value that indicates whether the content item is streaming content.

var playbackProgress: Float

The amount of content played for the media item.

var subtitle: String?

A secondary designator for the media item.

var title: String?

The public name of the media item.

