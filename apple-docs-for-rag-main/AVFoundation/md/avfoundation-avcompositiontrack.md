

- AVFoundation
-  AVCompositionTrack 

Class

# AVCompositionTrack

A track in a composition that presents media of a uniform type.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVCompositionTrack
```

## Overview

This object provides an immutable composition track. The framework also provides a mutable subclass, AVMutableCompositionTrack.

## Topics

### Accessing Track Information

var isPlayable: Bool

A Boolean value that indicates whether the track is playable in the current environment.

var isDecodable: Bool

A Boolean value that indicates whether the track is decodable in the current environment.

var isEnabled: Bool

A Boolean value that indicates whether the track’s container enables it.

var isSelfContained: Bool

A Boolean value that indicates whether this track references sample data only within its container file.

var totalSampleDataLength: Int64

The total number of bytes of sample data the track requires.

func hasMediaCharacteristic(AVMediaCharacteristic) -> Bool

Returns a Boolean value that indicates whether the track references media with the specified media characteristic.

### Accessing Temporal Information

var timeRange: CMTimeRange

The time range of the track within the overall timeline of the asset.

var naturalTimeScale: CMTimeScale

The natural time scale of the media that a track references.

var estimatedDataRate: Float

The estimated data rate, in bits per second, of the media that the track references.

func samplePresentationTime(forTrackTime: CMTime) -> CMTime

Maps the specified track time through the appropriate time mapping and returns the resulting sample presentation time.

### Accessing Language Support

var languageCode: String?

The language code of the track.

var extendedLanguageTag: String?

The language tag of the track.

### Managing Format Descriptions

var formatDescriptions: [Any]

The format descriptions of the media samples that a track references.

var formatDescriptionReplacements: [AVCompositionTrackFormatDescriptionReplacement]

The replacement format descriptions.

class AVCompositionTrackFormatDescriptionReplacement

An object that represents a format description and its replacement.

### Accessing Visual Characteristics

var naturalSize: CGSize

The natural dimensions of the media data that the track references.

var preferredTransform: CGAffineTransform

The track’s transform preference to apply to its visual content during presentation or processing.

### Accessing Audible Characteristics

var preferredVolume: Float

The track’s volume preference for playing its audible media.

var hasAudioSampleDependencies: Bool

A Boolean value that indicates whether the track has sample dependencies.

### Accessing Frame-Based Characteristics

var nominalFrameRate: Float

The frame rate of the track, in frames per second.

var minFrameDuration: CMTime

The minimum duration of the track’s frames.

var requiresFrameReordering: Bool

A Boolean value that indicates whether samples in the track may have different presentation and decode timestamps.

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers that have a value.

var commonMetadata: [AVMetadataItem]

An array of metadata items for all common metadata keys that have a value.

var availableMetadataFormats: [AVMetadataFormat]

An array of metadata formats available for the track.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns metadata items that a track contains for the specified format.

### Accessing Track Segments

var segments: [AVCompositionTrackSegment]

The time mappings from the track’s media samples to its timeline.

func segment(forTrackTime: CMTime) -> AVCompositionTrackSegment?

Returns a segment whose target time range contains, or is closest to, the specified track time.

### Accessing Track Associations

var availableTrackAssociationTypes: [AVAssetTrack.AssociationType]

An array of association types that the track uses to associate with other tracks.

func associatedTracks(ofType: AVAssetTrack.AssociationType) -> [AVAssetTrack]

Returns an array of associated tracks that have the specified association type.

### Determining Sample Cursor Support

var canProvideSampleCursors: Bool

A Boolean value that indicates whether the track can provide instances of sample cursors to traverse its media samples and discover information.

## Relationships

### Inherits From

- AVAssetTrack

### Inherited By

- AVMutableCompositionTrack

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

### Compositions

class AVComposition

An object that combines and arranges media from multiple assets into a single composite asset that you can play or process.

class AVCompositionTrackSegment

A track segment that maps a time from the source media track to the composition track.

