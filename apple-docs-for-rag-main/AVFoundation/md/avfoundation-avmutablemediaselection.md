

- AVFoundation
-  AVMutableMediaSelection 

Class

# AVMutableMediaSelection

A mutable object that represents a complete rendition of media selection options on an asset.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVMutableMediaSelection
```

## Topics

### Selecting Media Options

func select(AVMediaSelectionOption?, in: AVMediaSelectionGroup)

Selects the media option in the specified media selection group.

## Relationships

### Inherits From

- AVMediaSelection

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Media selection

Selecting Subtitles and Alternative Audio Tracks

Extend your app’s appeal to users by adding subtitles and alternative audio tracks in their native language.

class AVMediaSelection

An object that represents a complete rendition of media selection options on an asset.

class AVMediaSelectionGroup

An object that represents a collection of mutually exclusive options for the presentation of media within an asset.

class AVMediaSelectionOption

An object that represents a specific option for the presentation of media within a group of options.

class AVPlayerMediaSelectionCriteria

An object that specifies the preferred languages and media characteristics for a player.

