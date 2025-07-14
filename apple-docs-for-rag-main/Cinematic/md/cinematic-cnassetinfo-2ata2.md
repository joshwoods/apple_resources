

- Cinematic
-  CNAssetInfo 

Class

# CNAssetInfo

An object that provides Cinematic-specific information about an asset, including its tracks.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
class CNAssetInfo
```

## Topics

### Initializers

init(asset: AVAsset) async throws

Creates a Cinematic object from an asset.

### Instance Properties

var allCinematicTracks: [AVAssetTrack]

An array of the Cinematic asset tracks.

let asset: AVAsset

The original Cinematic source asset.

var cinematicDisparityTrack: AVAssetTrack

The Cinematic disparity track.

var cinematicMetadataTrack: AVAssetTrack

The Cinematic metadata track used.

var cinematicVideoTrack: AVAssetTrack

Track used for Cinematic video.

var frameTimingTrack: AVAssetTrack

The track used for Cinematic frame timing.

var naturalSize: CGSize

The video size if rendered at its natural size.

var preferredSize: CGSize

The video size if rendered at its natural size with the preferred transform applied.

var preferredTransform: CGAffineTransform

The preferred transform of the rendered image for display purposes.

var sampleDataTrackIDs: [CMPersistentTrackID]

The source metadata track IDs required to implement the video composition instruction protocol.

var timeRange: CMTimeRange

The time range over which all Cinematic tracks are valid.

var videoCompositionTrackIDs: [CMPersistentTrackID]

Source video track IDs required to implement the video composition instruction protocol.

var videoCompositionTracks: [AVAssetTrack]

Tracks required to construct the video composition output.

### Type Methods

class func isCinematic(asset: AVAsset) async -> Bool

Determines if the asset is Cinematic asynchronously.

## Relationships

### Inherited By

- CNCompositionInfo

## See Also

### Reading and rendering

class CNCompositionInfo

An object that enables you to add the appropriate number of tracks for a Cinematic asset.

class CNRenderingSession

An object representing the context in which rendering occurs.

