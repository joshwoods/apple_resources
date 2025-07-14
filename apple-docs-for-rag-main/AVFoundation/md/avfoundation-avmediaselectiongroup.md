

- AVFoundation
-  AVMediaSelectionGroup 

Class

# AVMediaSelectionGroup

An object that represents a collection of mutually exclusive options for the presentation of media within an asset.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMediaSelectionGroup
```

## Mentioned in 

Selecting Subtitles and Alternative Audio Tracks

## Topics

### Accessing Media Selection Options

var options: [AVMediaSelectionOption]

A collection of mutually exclusive media selection options

func mediaSelectionOption(withPropertyList: Any) -> AVMediaSelectionOption?

Returns the media selection options that match the given property list.

var defaultOption: AVMediaSelectionOption?

The default option in the group.

### Configuring Empty Selection Behavior

var allowsEmptySelection: Bool

A Boolean value that indicates whether it’s possible to present none of the options in the group when an associated player item is played.

### Filtering Selection Options

class func playableMediaSelectionOptions(from: [AVMediaSelectionOption]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that are playable.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], with: Locale) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that match the specified locale.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], withMediaCharacteristics: [AVMediaCharacteristic]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that match given media characteristics.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], withoutMediaCharacteristics: [AVMediaCharacteristic]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that do not match given media characteristics.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMediaSelectionOption]

Returns an array of media selection options, filtering them according to whether their locales match one of the specified languages.

### Creating a Now Playing Language Option Group

func makeNowPlayingInfoLanguageOptionGroup() -> MPNowPlayingInfoLanguageOptionGroup

Creates a language option group from the media selection group.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVAssetWriterInputGroup

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Media selection

Selecting Subtitles and Alternative Audio Tracks

Extend your app’s appeal to users by adding subtitles and alternative audio tracks in their native language.

class AVMediaSelection

An object that represents a complete rendition of media selection options on an asset.

class AVMediaSelectionOption

An object that represents a specific option for the presentation of media within a group of options.

class AVMutableMediaSelection

A mutable object that represents a complete rendition of media selection options on an asset.

class AVPlayerMediaSelectionCriteria

An object that specifies the preferred languages and media characteristics for a player.

