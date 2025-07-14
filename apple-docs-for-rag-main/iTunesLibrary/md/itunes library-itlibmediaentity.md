

- iTunes Library
-  ITLibMediaEntity 

Class

# ITLibMediaEntity

This class describes a media entity, which can be a media item, such as an audio track.

Mac Catalyst 14.0+macOS 10.13+

``` source
class ITLibMediaEntity
```

## Overview

Note

Entity properties are specific to each type of entity, and each specific entity class provides individual accessors for its properties.

Each media entity has a persistent unique ID and set of properties that iTunes assigns.

The `ITLibMediaEntity` class serves as the abstract superclass for ITLibMediaItem and ITLibPlaylist instances.

## Topics

### Essentials

var persistentID: NSNumber

The unique identifier of the media entity.

### Getting Media Item Properties

func enumerateValues(forProperties: Set&lt;String>?, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for the item properties.

func enumerateValuesExcept(forProperties: Set&lt;String>?, using: (String, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a provided block with the fetched values for all properties in the entity except for the provided set.

func value(forProperty: String) -> Any?

Gets the value for a specified media property key.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ITLibMediaItem
- ITLibPlaylist

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media Items

class ITLibMediaItem

This class describes a media item (a track) in the iTunes library, such as a song, a video, or a podcast.

class ITLibArtist

This class represents an artist, such as the performer of a song.

class ITLibArtwork

This class represents the artwork for a media item.

class ITLibMediaItemVideoInfo

This class encapsulates the video information of a video media item.

