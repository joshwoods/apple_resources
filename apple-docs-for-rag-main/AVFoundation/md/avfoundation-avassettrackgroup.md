

- AVFoundation
-  AVAssetTrackGroup 

Class

# AVAssetTrackGroup

A group of related tracks in an asset.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVAssetTrackGroup
```

## Overview

A track group describes a group of related alternative tracks, only one of which should play at a time. Groups of alternative tracks typically contain variations of the same content, like subtitles in multiple translations.

You can inspect an asset’s track groups by loading the value of its trackGroups property.

## Topics

### Getting Track ID Values

var trackIDs: [NSNumber]

The IDs of the tracks in the group.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Assets

class AVAsset

An object that models timed audiovisual media.

class AVURLAsset

An asset that represents media at a local or remote URL.

class AVAssetTrack

An object that models a track of media that an asset contains.

class AVAssetTrackSegment

An object that represents a time range segment of an asset track.

