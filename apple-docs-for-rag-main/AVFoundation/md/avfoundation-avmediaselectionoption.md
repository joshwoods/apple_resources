

- AVFoundation
-  AVMediaSelectionOption 

Class

# AVMediaSelectionOption

An object that represents a specific option for the presentation of media within a group of options.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMediaSelectionOption
```

## Mentioned in 

Selecting Subtitles and Alternative Audio Tracks

## Topics

### Accessing Media Information

var mediaType: AVMediaType

The media type of the media data.

var mediaSubTypes: [NSNumber]

The media sub-types of the media data associated with the option.

func hasMediaCharacteristic(AVMediaCharacteristic) -> Bool

Returns a Boolean value that indicates whether the receiver has media with the given media characteristic.

### Managing Metadata

var commonMetadata: [AVMetadataItem]

An array of metadata items for each common metadata key for which a value is available.

var availableMetadataFormats: [String]

The metadata formats that contain metadata associated with the option.

func metadata(forFormat: String) -> [AVMetadataItem]

Returns an array of metadata items—one for each metadata item in the container of a given format.

### Determining Playability

var isPlayable: Bool

A Boolean value that indicates whether the media selection option is playable.

### Getting the Language and Locale Settings

var displayName: String

A string suitable for display using the current system locale.

func displayName(with: Locale) -> String

Returns a string suitable for display using the specified locale.

var locale: Locale?

The locale for which the media option was authored.

var extendedLanguageTag: String?

The IETF BCP 47 language tag associated with the option

### Getting the Associated Media Selection Option

func associatedMediaSelectionOption(in: AVMediaSelectionGroup) -> AVMediaSelectionOption?

Returns a media selection option associated with the receiver in a given group.

### Creating a Now Playing Language Option

func makeNowPlayingInfoLanguageOption() -> MPNowPlayingInfoLanguageOption?

Creates a language option for a media selection option.

### Creating a Property List Representation

func propertyList() -> Any

Returns a serializable property list that’s sufficient to identify the option within its group.

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

## See Also

### Media selection

Selecting Subtitles and Alternative Audio Tracks

Extend your app’s appeal to users by adding subtitles and alternative audio tracks in their native language.

class AVMediaSelection

An object that represents a complete rendition of media selection options on an asset.

class AVMediaSelectionGroup

An object that represents a collection of mutually exclusive options for the presentation of media within an asset.

class AVMutableMediaSelection

A mutable object that represents a complete rendition of media selection options on an asset.

class AVPlayerMediaSelectionCriteria

An object that specifies the preferred languages and media characteristics for a player.

