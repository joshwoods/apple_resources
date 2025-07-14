

- AVFoundation
-  AVMutableMovieTrack 

Class

# AVMutableMovieTrack

A mutable track that conforms to the QuickTime or ISO base media file format.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
class AVMutableMovieTrack
```

## Topics

### Managing Time Ranges

func insertTimeRange(CMTimeRange, of: AVAssetTrack, at: CMTime, copySampleData: Bool) throws

Inserts a portion of an asset track into the target movie.

func insertEmptyTimeRange(CMTimeRange)

Adds an empty time range to a track.

func removeTimeRange(CMTimeRange)

Removes the specified time range from a track.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of a time range in a track.

### Appending Sample Data

func append(CMSampleBuffer, decodeTime: UnsafeMutablePointer&lt;CMTime>?, presentationTime: UnsafeMutablePointer&lt;CMTime>?) throws

Appends sample data to a media file and adds sample references for the added data to a track’s media sample tables.

func insertMediaTimeRange(CMTimeRange, into: CMTimeRange) -> Bool

Inserts a reference to a media time range into a track.

### Accessing Media Chunks

var preferredMediaChunkAlignment: Int

The boundary for media chunk alignment for file types that support media chunk alignment.

var preferredMediaChunkDuration: CMTime

The maximum duration to use for each chunk of sample data written to the file for file types that support media chunk duration.

var preferredMediaChunkSize: Int

The maximum size to use for each chunk of sample data written to the file for file types that support media chunk duration.

### Changing Format Descriptions

var formatDescriptions: [Any]

The format descriptions of the media samples that a track references.

func replaceFormatDescription(CMFormatDescription, with: CMFormatDescription)

Replaces the track’s format description with a new format description.

### Configuring Track Information

var isModified: Bool

A Boolean value that indicates whether a track is in a modified state.

var alternateGroupID: Int

A number that identifies the track as a member of a particular alternate group.

var mediaDataStorage: AVMediaDataStorage?

A storage container for the media data to be added to a track.

var sampleReferenceBaseURL: URL?

The base URL for sample references.

### Accessing Track Information

var isPlayable: Bool

A Boolean value that indicates whether the track is playable in the current environment.

var isDecodable: Bool

A Boolean value that indicates whether the track is decodable in the current environment.

var isEnabled: Bool

A Boolean value that indicates whether the track’s container enables it.

var isSelfContained: Bool

A Boolean value that indicates whether this track references sample data only within its container file.

var hasProtectedContent: Bool

A Boolean value that indicates whether a track contains protected content.

var totalSampleDataLength: Int64

The total number of bytes of sample data the track requires.

func hasMediaCharacteristic(AVMediaCharacteristic) -> Bool

Returns a Boolean value that indicates whether the track references media with the specified media characteristic.

### Accessing Temporal Information

var timeRange: CMTimeRange

The time range of the track within the overall timeline of the asset.

var timescale: CMTimeScale

The time scale for tracks that contain the `moov` atom.

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

### Accessing Visual Characteristics

var naturalSize: CGSize

The dimensions used to display the visual media data for the track.

var preferredTransform: CGAffineTransform

The transform performed on the visual media data of the track for display purposes.

var layer: Int

The layer level for the visual media of the track.

var cleanApertureDimensions: CGSize

The clean aperture dimension of the track.

var productionApertureDimensions: CGSize

The production aperture dimensions of the track.

var encodedPixelsDimensions: CGSize

The encoded pixels dimensions of the track.

### Accessing Audible Characteristics

var preferredVolume: Float

The preferred volume for the audible medata data of the track.

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

An array of metadata stored by the track.

var commonMetadata: [AVMetadataItem]

An array of metadata items for all common metadata keys that have a value.

var availableMetadataFormats: [AVMetadataFormat]

An array of metadata formats available for the track.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns metadata items that a track contains for the specified format.

### Accessing Track Segments

var segments: [AVAssetTrackSegment]

The time mappings from the track’s media samples to its timeline.

func segment(forTrackTime: CMTime) -> AVAssetTrackSegment?

Returns a segment whose target time range contains, or is closest to, the specified track time.

### Managing Track Associations

var availableTrackAssociationTypes: [AVAssetTrack.AssociationType]

An array of association types that the track uses to associate with other tracks.

func associatedTracks(ofType: AVAssetTrack.AssociationType) -> [AVAssetTrack]

Returns an array of associated tracks that have the specified association type.

func addTrackAssociation(to: AVMovieTrack, type: AVAssetTrack.AssociationType)

Creates a specific type of track association between two tracks.

func removeTrackAssociation(to: AVMovieTrack, type: AVAssetTrack.AssociationType)

Removes a specific type of track association between two tracks.

### Determining Sample Cursor Support

var canProvideSampleCursors: Bool

A Boolean value that indicates whether the track can provide instances of sample cursors to traverse its media samples and discover information.

## Relationships

### Inherits From

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

### Mutable movies

class AVMutableMovie

A mutable object that represents an audiovisual container that conforms to the QuickTime movie file format or a related format like MPEG-4.

