

- AVFoundation
- Media assets
- AVPartialAsyncProperty
-  AVAsset 

API Collection

# AVAsset

Asynchronous properties for assets.

## Topics

### Loading Duration and Timing

static var duration: AVAsyncProperty&lt;Root, CMTime>

A time value that represents the duration of the asset.

static var providesPreciseDurationAndTiming: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the asset provides precise duration and timing.

static var minimumTimeOffsetFromLive: AVAsyncProperty&lt;Root, CMTime>

A time value that indicates how closely playback follows the latest live stream content.

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVAssetTrack]>

The tracks of media that an asset contains.

### Loading Track Groups

static var trackGroups: AVAsyncProperty&lt;Root, [AVAssetTrackGroup]>

The track groups an asset contains.

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for all metadata identifiers.

static var commonMetadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

The metadata items that an asset contains for common metadata identifiers.

static var availableMetadataFormats: AVAsyncProperty&lt;Root, [AVMetadataFormat]>

The formats of metadata that an asset contains.

static var creationDate: AVAsyncProperty&lt;Root, AVMetadataItem?>

A metadata item that indicates the creation date of an asset.

static var lyrics: AVAsyncProperty&lt;Root, String?>

The lyrics of the asset in a language suitable for the current locale.

### Loading Suitability

static var isPlayable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether an asset contains playable content.

static var isExportable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can export an asset using an export session.

static var isReadable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

static var isComposable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can use the asset in a media composition.

static var isCompatibleWithSavedPhotosAlbum: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can write the asset to the Saved Photos album.

static var isCompatibleWithAirPlayVideo: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the asset is compatible with AirPlay Video.

### Loading Asset Preferences

static var preferredRate: AVAsyncProperty&lt;Root, Float>

The asset’s rate preference for playing its media.

static var preferredTransform: AVAsyncProperty&lt;Root, CGAffineTransform>

The asset’s transform preference to apply to its visual content during presentation or processing.

static var preferredVolume: AVAsyncProperty&lt;Root, Float>

The asset’s volume preference for playing its audible media.

static var preferredDisplayCriteria: AVAsyncProperty&lt;Root, AVDisplayCriteria>

The asset’s display mode preference for optimal playback of its content.

### Loading Media Selections

static var allMediaSelections: AVAsyncProperty&lt;Root, [AVMediaSelection]>

The available media selections for an asset.

static var preferredMediaSelection: AVAsyncProperty&lt;Root, AVMediaSelection>

The default media selections for the media selection groups of an asset.

static var availableMediaCharacteristicsWithMediaSelectionOptions: AVAsyncProperty&lt;Root, [AVMediaCharacteristic]>

The media characteristics that provide media selection options.

### Loading Chapter Metadata

static var availableChapterLocales: AVAsyncProperty&lt;Root, [Locale]>

The locales of an asset’s chapter metadata.

### Loading Content Protections

static var hasProtectedContent: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the asset contains protected content.

### Loading Fragment Support

static var canContainFragments: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can extend the asset by fragments.

static var containsFragments: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether at least one movie fragment extends the asset.

static var overallDurationHint: AVAsyncProperty&lt;Root, CMTime>

A hint to the total duration of fragments that currently exist or may exist in the future.

## See Also

### Loading Properties

AVAssetTrack

Asynchronous properties for asset tracks.

AVURLAsset

Asynchronous properties for URL assets.

AVFragmentedAsset

Asynchronous properties for fragmented assets.

AVMetadataItem

Asynchronous properties for metadata items.

AVComposition

Asynchronous properties for compositions.

AVMutableComposition

Asynchronous properties for mutable compositions.

AVMovie

Asynchronous properties for movies.

AVMutableMovie

Asynchronous properties for mutable movies.

AVFragmentedMovie

Asynchronous properties for fragmented movies.

