

- AVFoundation
- Media assets
- AVAssetTrack
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Overview

AVAssetTrack doesn’t support using its synchronous property accessors that can block the calling thread. Instead, use the load(_:) method to load AVAsyncProperty values asynchronously.

## Topics

### Accessing Track Information

var formatDescriptions: [Any]

The format descriptions of the media samples that a track references.

Deprecated

var isPlayable: Bool

A Boolean value that indicates whether the track is playable in the current environment.

Deprecated

var isDecodable: Bool

A Boolean value that indicates whether the track is decodable in the current environment.

Deprecated

var isEnabled: Bool

A Boolean value that indicates whether the track’s container enables it.

Deprecated

var isSelfContained: Bool

A Boolean value that indicates whether this track references sample data only within its container file.

Deprecated

var totalSampleDataLength: Int64

The total number of bytes of sample data the track requires.

Deprecated

func hasMediaCharacteristic(AVMediaCharacteristic) -> Bool

Returns a Boolean value that indicates whether the track references media with the specified media characteristic.

Deprecated

### Accessing Temporal Information

var timeRange: CMTimeRange

The time range of the track within the overall timeline of the asset.

Deprecated

var naturalTimeScale: CMTimeScale

The natural time scale of the media that a track references.

Deprecated

var estimatedDataRate: Float

The estimated data rate, in bits per second, of the media that the track references.

Deprecated

### Accessing Language Support

var languageCode: String?

The language code of the track.

Deprecated

var extendedLanguageTag: String?

The language tag of the track.

Deprecated

### Accessing Visual Characteristics

var naturalSize: CGSize

The natural dimensions of the media data that the track references.

Deprecated

var preferredTransform: CGAffineTransform

The track’s transform preference to apply to its visual content during presentation or processing.

Deprecated

### Accessing Audible Characteristics

var preferredVolume: Float

The track’s volume preference for playing its audible media.

Deprecated

var hasAudioSampleDependencies: Bool

A Boolean value that indicates whether the track has sample dependencies.

Deprecated

### Accessing Frame-Based Characteristics

var nominalFrameRate: Float

The frame rate of the track, in frames per second.

Deprecated

var minFrameDuration: CMTime

The minimum duration of the track’s frames.

Deprecated

var requiresFrameReordering: Bool

A Boolean value that indicates whether samples in the track may have different presentation and decode timestamps.

Deprecated

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers that have a value.

Deprecated

var commonMetadata: [AVMetadataItem]

An array of metadata items for all common metadata keys that have a value.

Deprecated

var availableMetadataFormats: [AVMetadataFormat]

An array of metadata formats available for the track.

Deprecated

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns metadata items that a track contains for the specified format.

Deprecated

### Accessing Track Segments

var segments: [AVAssetTrackSegment]

The time mappings from the track’s media samples to its timeline.

Deprecated

func segment(forTrackTime: CMTime) -> AVAssetTrackSegment?

Retrieves a segment with a target time range that contains, or is closest to, the specified track time.

Deprecated

func samplePresentationTime(forTrackTime: CMTime) -> CMTime

Maps the specified track time through the appropriate time mapping and returns the resulting sample presentation time.

Deprecated

### Accessing Track Associations

var availableTrackAssociationTypes: [AVAssetTrack.AssociationType]

An array of association types that the track uses to associate with other tracks.

Deprecated

func associatedTracks(ofType: AVAssetTrack.AssociationType) -> [AVAssetTrack]

Returns an array of associated tracks that have the specified association type.

Deprecated

### Creating Sample Cursors

var canProvideSampleCursors: Bool

A Boolean value that indicates whether the track can provide instances of sample cursors to traverse its media samples and discover information.

Deprecated

