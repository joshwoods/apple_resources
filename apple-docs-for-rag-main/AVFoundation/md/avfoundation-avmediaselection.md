

- AVFoundation
-  AVMediaSelection 

Class

# AVMediaSelection

An object that represents a complete rendition of media selection options on an asset.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVMediaSelection
```

## Topics

### Inspecting the Media Selection

func selectedMediaOption(in: AVMediaSelectionGroup) -> AVMediaSelectionOption?

Returns the media selection option that’s currently selected in the specified group.

func mediaSelectionCriteriaCanBeAppliedAutomatically(to: AVMediaSelectionGroup) -> Bool

Indicates whether the specified media selection group is subject to automatic media selection.

### Accessing the Asset

var asset: AVAsset?

The asset associated with the media selection.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableMediaSelection

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

class AVMediaSelectionGroup

An object that represents a collection of mutually exclusive options for the presentation of media within an asset.

class AVMediaSelectionOption

An object that represents a specific option for the presentation of media within a group of options.

class AVMutableMediaSelection

A mutable object that represents a complete rendition of media selection options on an asset.

class AVPlayerMediaSelectionCriteria

An object that specifies the preferred languages and media characteristics for a player.

