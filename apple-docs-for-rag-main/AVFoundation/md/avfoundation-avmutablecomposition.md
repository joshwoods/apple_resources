

- AVFoundation
-  AVMutableComposition 

Class

# AVMutableComposition

An object that you use to create a new composition from existing assets.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMutableComposition
```

## Overview

Use this object to add and remove composition tracks, and add, remove, and scale their time ranges. You can make an immutable snapshot of a mutable composition for playback and inspection as follows:

```
// Use a mutable composition object you create.
let mutableComposition = AVMutableComposition()

guard let composition = mutableComposition.copy() as? AVComposition else { return }

// Create a player item to inspect and play the composition.
let playerItem = AVPlayerItem(asset: composition)
```

## Topics

### Creating a Composition

convenience init(urlAssetInitializationOptions: [String : Any]?)

Creates a mutable composition that uses the specified initialization options.

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVMutableCompositionTrack]>

The tracks that a composition contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVMutableCompositionTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVMutableCompositionTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVMutableCompositionTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

### Accessing Tracks

Prefer loading tracks asynchronously using the methods in Loading Tracks.

var tracks: [AVMutableCompositionTrack]

The tracks that a composition contains.

func track(withTrackID: CMPersistentTrackID) -> AVMutableCompositionTrack?

Returns a track that contains the specified identifier.

func tracks(withMediaType: AVMediaType) -> [AVMutableCompositionTrack]

Returns tracks that contain media of a specified type.

func tracks(withMediaCharacteristic: AVMediaCharacteristic) -> [AVMutableCompositionTrack]

Returns tracks that contain media of a specified characteristic.

### Managing Composition Tracks

func mutableTrack(compatibleWith: AVAssetTrack) -> AVMutableCompositionTrack?

Returns a composition track into which you can insert any time range of the specified asset track.

func addMutableTrack(withMediaType: AVMediaType, preferredTrackID: CMPersistentTrackID) -> AVMutableCompositionTrack?

Adds an empty track to a composition.

func removeTrack(AVCompositionTrack)

Removes a specified track from the composition.

### Managing Cinematic Tracks

func addTracks(for: CNAssetInfo, preferredStartingTrackID: CMPersistentTrackID) -> CNCompositionInfo

### Managing Time Ranges

func removeTimeRange(CMTimeRange)

Removes a specified time range from all tracks of the composition.

func scaleTimeRange(CMTimeRange, toDuration: CMTime)

Changes the duration of all tracks in a given time range.

func insertEmptyTimeRange(CMTimeRange)

Adds or extends an empty time range within all tracks of the composition.

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, completionHandler: ((any Error)?) -> Void)

Inserts all tracks of an asset for a time range into a composition.

Deprecated

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime) throws

Inserts all the tracks within a given time range of a specified asset into the composition.

Deprecated

### Configuring Video Size

var naturalSize: CGSize

The encoded or authored size of the visual portion of the asset.

### Instance Methods

func insertTimeRange(CMTimeRange, of: AVAsset, at: CMTime, isolation: isolated (any Actor)?) async throws

## Relationships

### Inherits From

- AVComposition

### Conforms To

- AVAsynchronousKeyValueLoading
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Mutable compositions

class AVMutableCompositionTrack

A mutable track in a composition that you use to insert, remove, and scale track segments without affecting their low-level representation.

