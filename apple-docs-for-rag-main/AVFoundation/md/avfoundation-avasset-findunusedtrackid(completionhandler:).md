

- AVFoundation
- AVAsset
-  findUnusedTrackID(completionHandler:) 

Instance Method

# findUnusedTrackID(completionHandler:)

Loads an identifier that no other track in the asset uses.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func findUnusedTrackID(completionHandler: @escaping (CMPersistentTrackID, (any Error)?) -> Void)
```

``` source
func findUnusedTrackID() async throws -> CMPersistentTrackID
```

## Parameters 

`completionHandler`  

A completion handler the system calls after it finishes the request.

## See Also

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVAssetTrack]>

The tracks of media that an asset contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVAssetTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVAssetTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVAssetTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

