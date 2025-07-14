

- AVFoundation
- Media assets
- AVAsset
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Overview

AVAsset doesn’t support using its synchronous property accessors that can block the calling thread. Instead, use the load(_:) method to load AVAsyncProperty values asynchronously.

## Topics

### Accessing Duration and Timing

var duration: CMTime

A time value that indicates the asset’s duration.

Deprecated

var providesPreciseDurationAndTiming: Bool

A Boolean value that indicates whether the asset provides precise duration and timing.

Deprecated

var minimumTimeOffsetFromLive: CMTime

A time value that indicates how closely playback follows the latest live stream content.

Deprecated

### Accessing Tracks

var tracks: [AVAssetTrack]

The tracks an asset contains.

Deprecated

func track(withTrackID: CMPersistentTrackID) -> AVAssetTrack?

Returns a track that contains the specified identifier.

Deprecated

func tracks(withMediaType: AVMediaType) -> [AVAssetTrack]

Returns tracks that contain media of a specified type.

Deprecated

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVAssetTrack]

Returns an array of asset tracks matching the specified media characteristic.

Deprecated

func unusedTrackID() -> CMPersistentTrackID

Returns an identifier that no other tracks in the asset use.

Deprecated

### Accessing Track Groups

var trackGroups: [AVAssetTrackGroup]

The track groups an asset contains.

Deprecated

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers for which a value is available.

Deprecated

var commonMetadata: [AVMetadataItem]

The metadata items an asset contains for common metadata identifiers that provide a value.

Deprecated

var availableMetadataFormats: [AVMetadataFormat]

The metadata formats this asset contains.

Deprecated

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns an array of metadata items from the container with the specified format.

Deprecated

var creationDate: AVMetadataItem?

A metadata item that indicates the asset’s creation date.

Deprecated

var lyrics: String?

The lyrics of the asset in a language suitable for the current locale.

Deprecated

### Accessing Suitability

var isPlayable: Bool

A Boolean value that indicates whether the asset has playable content.

Deprecated

var isExportable: Bool

A Boolean value that indicates whether you can export this asset using an export session.

Deprecated

var isReadable: Bool

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

Deprecated

var isComposable: Bool

A Boolean value that indicates whether you can use the asset as a segment of a composition track.

Deprecated

var isCompatibleWithAirPlayVideo: Bool

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

Deprecated

var isCompatibleWithSavedPhotosAlbum: Bool

A Boolean value that indicates whether you can write the asset to the Saved Photos album.

Deprecated

### Accessing Asset Preferences

Prefer loading access preferences asynchronously using the properties in Loading Asset Preferences.

var preferredRate: Float

The asset’s rate preference for playing its media.

Deprecated

var preferredVolume: Float

The asset’s volume preference for playing its audible media.

Deprecated

var preferredTransform: CGAffineTransform

The asset’s transform preference to apply to its visual content during presentation or processing.

Deprecated

var preferredDisplayCriteria: AVDisplayCriteria

The asset’s display mode preference for optimal playback of its content.

Deprecated

var preferredMediaSelection: AVMediaSelection

The default media selections for this asset’s media selection groups.

Deprecated

### Accessing Media Selections

var allMediaSelections: [AVMediaSelection]

The array of available media selections for this asset.

Deprecated

var availableMediaCharacteristicsWithMediaSelectionOptions: [AVMediaCharacteristic]

An array of media characteristics for which a media selection option is available.

Deprecated

func mediaSelectionGroup(forMediaCharacteristic: AVMediaCharacteristic) -> AVMediaSelectionGroup?

Returns a media selection group that contains one or more options with the specified media characteristic.

Deprecated

### Accessing Chapter Metadata

var availableChapterLocales: [Locale]

The locales of the asset’s chapter metadata.

Deprecated

func chapterMetadataGroups(withTitleLocale: Locale, containingItemsWithCommonKeys: [AVMetadataKey]?) -> [AVTimedMetadataGroup]

Returns an array of chapters that contain the specified title locale and common keys.

Deprecated

func chapterMetadataGroups(bestMatchingPreferredLanguages: [String]) -> [AVTimedMetadataGroup]

Returns an array of chapters with a locale that best matches the list of preferred languages.

Deprecated

### Accessing Content Protections

var hasProtectedContent: Bool

A Boolean value that indicates whether the asset contains protected content.

Deprecated

### Accessing Fragment Support

var canContainFragments: Bool

A Boolean value that indicates whether you can extend the asset by fragments.

Deprecated

var containsFragments: Bool

A Boolean value that indicates whether at least one movie fragment extends the asset.

Deprecated

var overallDurationHint: CMTime

The total duration of fragments that currently exist, or may exist in the future.

Deprecated

### Inspecting Visual Attributes

var naturalSize: CGSize

The encoded or authored size of the visual portion of the asset.

Deprecated

