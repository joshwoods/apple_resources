

- Media Player
- MPContentItem
-  identifier 

Instance Property

# identifier

The unique identifier for the media item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+

``` source
var identifier: String { get }
```

## Discussion

All media items must have a unique identifier. Identifiers must be unique so that Media Player can properly update existing media items or add new media items. Media items won’t update properly if multiple media items have the same identifier.

## See Also

### Related Documentation

init(identifier: String)

Sets the identifier for a media item.

### Retrieving information about a media item

var artwork: MPMediaItemArtwork?

A single image that’s associated with the media item.

var isContainer: Bool

A Boolean value that indicates whether a media item is container of other items.

var isExplicitContent: Bool

A Boolean value that indicates whether the media item contains explicit content.

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

