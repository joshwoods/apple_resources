

- Media Player
-  MPMediaItemCollection 

Class

# MPMediaItemCollection

A sorted set of media items from the media library.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class MPMediaItemCollection
```

## Overview

Typically, you use this class by requesting an array of collections from a media query by way of its collections property. MPMediaQuery describes media queries.

The grouping type for the media query determines the arrangement of the media items you obtain. You also use the media query collections property to obtain synced playlists, as described in MPMediaPlaylist.

A media item collection can have a wide range of metadata associated with it. You access this metadata using the value(forProperty:) method along with the property keys described in this document. You can also access metadata in a batch fashion using the enumerateValues(forProperties:using:) method. In some cases, this is more efficient. MPMediaEntity defines and describes both of these methods.

## Topics

### Creating a media item collection

init(items: [MPMediaItem])

Initializes a media item collection with an array of media items.

### Using a media item collection

var items: [MPMediaItem]

The media items in a media item collection.

var representativeItem: MPMediaItem?

A media item whose properties are representative of the other media items in a collection.

var count: Int

The number of media items in a collection.

var mediaTypes: MPMediaType

The types of the media items in a collection.

## Relationships

### Inherits From

- MPMediaEntity

### Inherited By

- MPMediaPlaylist

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Media items and playlists

class MPMediaItem

A collection of properties that represents a single item in the media library.

class MPMediaItemArtwork

A graphical image, such as music album cover art, associated with a media item.

class MPMediaPlaylist

A playable collection of related media items.

class MPMediaPlaylistCreationMetadata

A set of attributes for describing a playlist when creating it.

class MPMediaEntity

The abstract superclass for media items, media item collections, and media playlist instances.

