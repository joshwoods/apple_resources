

- Media Player
-  MPContentItem 

Class

# MPContentItem

An object that contains the information for a displayed media item.

iOS 7.1+iPadOS 7.1+Mac Catalyst 13.1+macOS 10.12.2+tvOS 7.1+visionOS 1.0+

``` source
class MPContentItem
```

## Overview

This object represents a media item such as a song, movie, radio station, or podcast episode. The media player displays the information stored in it.

Update this object by changing its properties during runtime or by creating a new `MPContentItem` object with new property values, but with the same identifier as the object to change. Use the beginUpdates() and endUpdates() methods found in MPPlayableContentManager to update several `MPContentItem` objects at once.

Important

This class is only used for CarPlay. Using it requires a special entitlement issued by Apple. Apps without the correct entitlement won’t appear on the CarPlay home screen. See http://www.apple.com/ios/carplay/ for more information.

## Topics

### Setting a unique identifier

init(identifier: String)

Sets the identifier for a media item.

### Retrieving information about a media item

var artwork: MPMediaItemArtwork?

A single image that’s associated with the media item.

var isContainer: Bool

A Boolean value that indicates whether a media item is container of other items.

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

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

