

- AVFoundation
- Media assets
- AVPartialAsyncProperty
-  AVAssetTrack 

API Collection

# AVAssetTrack

Asynchronous properties for asset tracks.

## Topics

### Loading Track Information

static var totalSampleDataLength: AVAsyncProperty&lt;Root, Int64>

The total number of bytes of sample data the track requires.

static var formatDescriptions: AVAsyncProperty&lt;Root, [CMFormatDescription]>

The format descriptions of the media samples that a track references.

static var isDecodable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is decodable in the current environment.

static var isEnabled: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is in an enabled state.

static var isPlayable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is playable in the current environment.

static var mediaCharacteristics: AVAsyncProperty&lt;Root, [AVMediaCharacteristic]>

The media characteristics for the track.

static var isSelfContained: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track references sample data only within its container file.

### Loading Temporal Information

static var timeRange: AVAsyncProperty&lt;Root, CMTimeRange>

The time range of the track within the overall timeline of the asset.

static var naturalTimeScale: AVAsyncProperty&lt;Root, CMTimeScale>

The natural time scale of the media that a track references.

static var estimatedDataRate: AVAsyncProperty&lt;Root, Float>

The estimated data rate, in bits per second, of the media that the track references.

### Loading Language Support

static var languageCode: AVAsyncProperty&lt;Root, String?>

The language code of the track.

static var extendedLanguageTag: AVAsyncProperty&lt;Root, String?>

The language tag of the track.

### Loading Visual Characteristics

static var naturalSize: AVAsyncProperty&lt;Root, CGSize>

The natural dimensions of the media data that the track references.

static var preferredTransform: AVAsyncProperty&lt;Root, CGAffineTransform>

The track’s transform preference to apply to its visual content during presentation or processing.

### Loading Audible Characteristics

static var preferredVolume: AVAsyncProperty&lt;Root, Float>

The track’s volume preference for playing its audible media.

static var hasAudioSampleDependencies: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track has sample dependencies.

### Loading Frame-Based Characteristics

static var nominalFrameRate: AVAsyncProperty&lt;Root, Float>

The frame rate of the track, in frames per second.

static var minFrameDuration: AVAsyncProperty&lt;Root, CMTime>

The minimum duration of the track’s frames.

static var requiresFrameReordering: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether samples in the track may have different presentation and decode timestamps.

### Loading Metadata

static var metadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

An array of metadata items for all metadata identifiers that have a value.

static var availableMetadataFormats: AVAsyncProperty&lt;Root, [AVMetadataFormat]>

An array of metadata formats available for the track.

static var commonMetadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

An array of metadata items for all common metadata keys that have a value.

### Loading Track Segments

static var segments: AVAsyncProperty&lt;Root, [AVAssetTrackSegment]>

The time mappings from the track’s media samples to its timeline.

### Loading Track Associations

static var availableTrackAssociationTypes: AVAsyncProperty&lt;Root, [AVAssetTrack.AssociationType]>

An array of association types that the track uses to associate with other tracks.

### Creating Sample Cursors

static var canProvideSampleCursors: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track can provide instances of sample cursors to traverse its media samples and discover information.

## See Also

### Loading Properties

AVAsset

Asynchronous properties for assets.

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

