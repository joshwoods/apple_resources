

- AVFoundation
- AVMetadataIdentifier
-  quickTimeMetadataFullFrameRatePlaybackIntent 

Type Property

# quickTimeMetadataFullFrameRatePlaybackIntent

An identifier that represents whether this movie should play at full frame rate.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static let quickTimeMetadataFullFrameRatePlaybackIntent: AVMetadataIdentifier
```

## Discussion

Some apps play movies recorded at frame rates of 120fps or higher in slow motion. If your app records high-frame-rate movies, you can add this movie-level metadata to indicate whether the movie intends to play at the full frame rate (1) or at a slow motion rate (0). Apps that play movies may use this metadata, when present, to guide their behavior.

## See Also

### QuickTime Metadata Identifiers

static let quickTimeMetadataAccessibilityDescription: AVMetadataIdentifier

An identifier that represents the accessibility description for the movie file content.

static let quickTimeMetadataAlbum: AVMetadataIdentifier

An identifier that represents the name of the album or collection in QuickTime.

static let quickTimeMetadataArranger: AVMetadataIdentifier

An identifier that represents the name of the arranger of the movie file content.

static let quickTimeMetadataArtist: AVMetadataIdentifier

An identifier that represents the name of the artist of the movie file content.

static let quickTimeMetadataArtwork: AVMetadataIdentifier

An identifier that represents an image relating to the movie file content.

static let quickTimeMetadataAuthor: AVMetadataIdentifier

An identifier that represents the name of the author of the movie file content.

static let quickTimeMetadataAutoLivePhoto: AVMetadataIdentifier

An identifier that represents whether the live photo movie used auto mode.

static let quickTimeMetadataCameraFrameReadoutTime: AVMetadataIdentifier

An identifier that represents the camera frame readout time in QuickTime.

static let quickTimeMetadataCameraIdentifier: AVMetadataIdentifier

An identifier that represents the camera identifier in QuickTime.

static let quickTimeMetadataCollectionUser: AVMetadataIdentifier

An identifier that represents a name that indicates a user-defined collection.

static let quickTimeMetadataComment: AVMetadataIdentifier

An identifier that represents a comment regarding the movie file content.

static let quickTimeMetadataComposer: AVMetadataIdentifier

An identifier that represents the name of the composer of the movie file content.

static let quickTimeMetadataContentIdentifier: AVMetadataIdentifier

An identifier that represents the content identifier in QuickTime.

static let quickTimeMetadataCopyright: AVMetadataIdentifier

An identifier that represents the copyright statement for the movie file content.

static let quickTimeMetadataCreationDate: AVMetadataIdentifier

An identifier that represents the creation date of the movie file content.

