

- AVFoundation
- AVMetadataIdentifier
-  quickTimeMetadataLivePhotoVitalityScore 

Type Property

# quickTimeMetadataLivePhotoVitalityScore

An identifier that represents the vitality score of the Live Photo movie.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let quickTimeMetadataLivePhotoVitalityScore: AVMetadataIdentifier
```

## Discussion

Live Photo movies may be algorithmically scored from `0.0` to `1.0` on their level of vitality. A Live Photo movie with a low vitality score offers little dynamism to the still photo it accompanies. The vitality score is normalized and independent of the vitality scoring version of the algorithm defined by quickTimeMetadataLivePhotoVitalityScoringVersion.

If a Live Photo movie contains the quickTimeMetadataAutoLivePhoto key and its value is nonzero, apps should read the quickTimeMetadataLivePhotoVitalityScore value and only display the movie’s content if the score is `0.5` or higher.

If the capture session includes a metadata output configured to provide face, dog, or cat metadata objects, their presence greatly increases the vitality score.

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

