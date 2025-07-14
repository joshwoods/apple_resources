

- AVFoundation
-  AVComposition 

Class

# AVComposition

An object that combines and arranges media from multiple assets into a single composite asset that you can play or process.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVComposition
```

## Overview

A composition is a container for one or more tracks of media. Its tracks are instances of AVCompositionTrack that present media of a uniform type like audio or video. A track itself is a container for one or more segments of media, which are instances of AVCompositionTrackSegment, a type that represents a region of media in the source track.

## Topics

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVCompositionTrack]>

The tracks that a composition contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVCompositionTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVCompositionTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVCompositionTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

### Accessing Tracks

Prefer loading tracks asynchronously using the methods in Loading Tracks.

var tracks: [AVCompositionTrack]

The tracks that a composition contains.

func track(withTrackID: CMPersistentTrackID) -> AVCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVCompositionTrack]

Returns tracks that contain media of a specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVCompositionTrack]

Returns tracks that contain media of a specified characteristic.

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

### Accessing Track Groups

var trackGroups: [AVAssetTrackGroup]

The track groups an asset contains.

### Accessing Duration and Timing

var duration: CMTime

A time value that indicates the asset’s duration.

var providesPreciseDurationAndTiming: Bool

A Boolean value that indicates whether the asset provides precise duration and timing.

var minimumTimeOffsetFromLive: CMTime

A time value that indicates how closely playback follows the latest live stream content.

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers for which a value is available.

var commonMetadata: [AVMetadataItem]

The metadata items an asset contains for common metadata identifiers that provide a value.

var availableMetadataFormats: [AVMetadataFormat]

The metadata formats this asset contains.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns an array of metadata items from the container with the specified format.

var creationDate: AVMetadataItem?

A metadata item that indicates the asset’s creation date.

var lyrics: String?

The lyrics of the asset in a language suitable for the current locale.

### Determining Suitability

var isPlayable: Bool

A Boolean value that indicates whether the asset has playable content.

var isReadable: Bool

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

var isExportable: Bool

A Boolean value that indicates whether you can export this asset using an export session.

var isComposable: Bool

A Boolean value that indicates whether you can use the asset as a segment of a composition track.

var isCompatibleWithAirPlayVideo: Bool

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

var isCompatibleWithSavedPhotosAlbum: Bool

A Boolean value that indicates whether you can write the composition to the Saved Photos album.

### Inspecting Preferences

var preferredRate: Float

The asset’s rate preference for playing its media.

var preferredVolume: Float

The asset’s volume preference for playing its audible media.

var preferredTransform: CGAffineTransform

The asset’s transform preference to apply to its visual content during presentation or processing.

var preferredMediaSelection: AVMediaSelection

The default media selections for this asset’s media selection groups.

var preferredDisplayCriteria: AVDisplayCriteria

The asset’s display mode preference for optimal playback of its content.

### Accessing Media Selections

var allMediaSelections: [AVMediaSelection]

The array of available media selections for this asset.

var availableMediaCharacteristicsWithMediaSelectionOptions: [AVMediaCharacteristic]

An array of media characteristics for which a media selection option is available.

func mediaSelectionGroup(forMediaCharacteristic: AVMediaCharacteristic) -> AVMediaSelectionGroup?

Returns a media selection group that contains one or more options with the specified media characteristic.

### Accessing Chapter Metadata

var availableChapterLocales: [Locale]

The locales of the asset’s chapter metadata.

func chapterMetadataGroups(bestMatchingPreferredLanguages: [String]) -> [AVTimedMetadataGroup]

Returns an array of chapters with a locale that best matches the list of preferred languages.

func chapterMetadataGroups(withTitleLocale: Locale, containingItemsWithCommonKeys: [AVMetadataKey]?) -> [AVTimedMetadataGroup]

Returns an array of chapters that contain the specified title locale and common keys.

### Accessing Visual Dimensions

var naturalSize: CGSize

The authored size of the visual portion of the composition.

### Accessing Initialization Options

var urlAssetInitializationOptions: [String : Any]

The options you used to create a composition.

### Determining Content Protections

var hasProtectedContent: Bool

A Boolean value that indicates whether the asset contains protected content.

### Determining Fragment Support

var canContainFragments: Bool

A Boolean value that indicates whether you can extend the asset by fragments.

var containsFragments: Bool

A Boolean value that indicates whether at least one movie fragment extends the asset.

var overallDurationHint: CMTime

The total duration of fragments that currently exist, or may exist in the future.

## Relationships

### Inherits From

- AVAsset

### Inherited By

- AVMutableComposition

### Conforms To

- AVAsynchronousKeyValueLoading
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Compositions

class AVCompositionTrack

A track in a composition that presents media of a uniform type.

class AVCompositionTrackSegment

A track segment that maps a time from the source media track to the composition track.

