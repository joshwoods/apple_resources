

- AVFoundation
-  AVAssetTrack 

Class

# AVAssetTrack

An object that models a track of media that an asset contains.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVAssetTrack
```

## Mentioned in 

Loading media data asynchronously

Tagging Media with Video Color Information

## Overview

An asset contains one or more tracks of media that the framework models using the AVAssetTrack class. A track object holds the uniformly typed media that an asset provides such as audio, video, or closed captions.

A track, like its containing AVAsset, doesn’t load all of its media upon creation. Instead, it defers loading its data until you perform an operation that requires it. Because loading the data can take time, an asset track adopts the AVAsynchronousKeyValueLoading protocol so you can load its property values asynchronously by calling the load(_:) method.

## Topics

### Identifying an Asset Track

var trackID: CMPersistentTrackID

The persistent unique identifier for this track.

var mediaType: AVMediaType

The type of media that a track presents.

var asset: AVAsset?

The asset object that contains this track.

### Loading Track Information

static var formatDescriptions: AVAsyncProperty&lt;Root, [CMFormatDescription]>

The format descriptions of the media samples that a track references.

static var isPlayable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is playable in the current environment.

static var isDecodable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is decodable in the current environment.

static var isEnabled: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is in an enabled state.

static var isSelfContained: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track references sample data only within its container file.

static var totalSampleDataLength: AVAsyncProperty&lt;Root, Int64>

The total number of bytes of sample data the track requires.

static var mediaCharacteristics: AVAsyncProperty&lt;Root, [AVMediaCharacteristic]>

The media characteristics for the track.

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

static var commonMetadata: AVAsyncProperty&lt;Root, [AVMetadataItem]>

An array of metadata items for all common metadata keys that have a value.

static var availableMetadataFormats: AVAsyncProperty&lt;Root, [AVMetadataFormat]>

An array of metadata formats available for the track.

func loadMetadata(for: AVMetadataFormat, completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads metadata items that a track contains for the specified format.

### Loading Track Segments

static var segments: AVAsyncProperty&lt;Root, [AVAssetTrackSegment]>

The time mappings from the track’s media samples to its timeline.

func loadSegment(forTrackTime: CMTime, completionHandler: (AVAssetTrackSegment?, (any Error)?) -> Void)

Loads a segment with a target time range that contains, or is closest to, the specified track time.

func loadSamplePresentationTime(forTrackTime: CMTime, completionHandler: (CMTime, (any Error)?) -> Void)

Loads a sample presentation time that maps to the specified track time.

class AVAssetTrackSegment

An object that represents a time range segment of an asset track.

### Loading Track Associations

static var availableTrackAssociationTypes: AVAsyncProperty&lt;Root, [AVAssetTrack.AssociationType]>

An array of association types that the track uses to associate with other tracks.

func loadAssociatedTracks(ofType: AVAssetTrack.AssociationType, completionHandler: ([AVAssetTrack]?, (any Error)?) -> Void)

Loads associated tracks that have the specified association type.

### Creating Sample Cursors

func makeSampleCursor(presentationTimeStamp: CMTime) -> AVSampleCursor?

Creates a sample cursor and positions it at or near the specified presentation timestamp.

func makeSampleCursorAtFirstSampleInDecodeOrder() -> AVSampleCursor?

Creates a sample cursor and positions it at the track’s first media sample in decode order.

func makeSampleCursorAtLastSampleInDecodeOrder() -> AVSampleCursor?

Creates a sample cursor and positions it at the track’s last media sample in decode order.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCompositionTrack
- AVFragmentedAssetTrack
- AVMovieTrack

### Conforms To

- AVAsynchronousKeyValueLoading
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Assets

class AVAsset

An object that models timed audiovisual media.

class AVURLAsset

An asset that represents media at a local or remote URL.

class AVAssetTrackSegment

An object that represents a time range segment of an asset track.

class AVAssetTrackGroup

A group of related tracks in an asset.

