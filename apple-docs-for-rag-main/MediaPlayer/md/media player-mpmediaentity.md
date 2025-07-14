

- Media Player
-  MPMediaEntity 

Class

# MPMediaEntity

The abstract superclass for media items, media item collections, and media playlist instances.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
class MPMediaEntity
```

## Overview

This is the superclass for MPMediaItem and MPMediaItemCollection instances, and in turn for MPMediaPlaylist instances.

## Topics

### Working with media properties

class func canFilter(byProperty: String) -> Bool

Indicates whether you can use the media property key that you specify to construct a media property predicate.

func enumerateValues(forProperties: Set&lt;String>, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for the given item properties.

var persistentID: MPMediaEntityPersistentID

The persistent identifier for a media entity.

subscript(Any) -> Any?

Returns the object specified by the key.

func value(forProperty: String) -> Any?

Retrieves the value for a specified media property key.

typealias MPMediaEntityPersistentID

Defines the type for storing a persistent identifier to a particular entity.

### Media entity property keys

Media entity property keys

The property keys used to retrieve metadata for media entities.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MPMediaItem
- MPMediaItemCollection

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

class MPMediaItemCollection

A sorted set of media items from the media library.

class MPMediaPlaylist

A playable collection of related media items.

class MPMediaPlaylistCreationMetadata

A set of attributes for describing a playlist when creating it.

