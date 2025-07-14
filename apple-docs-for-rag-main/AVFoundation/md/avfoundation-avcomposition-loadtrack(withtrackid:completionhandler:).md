

- AVFoundation
- AVComposition
-  loadTrack(withTrackID:completionHandler:) 

Instance Method

# loadTrack(withTrackID:completionHandler:)

Loads a track that contains the specified identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadTrack(
    withTrackID trackID: CMPersistentTrackID,
    completionHandler: @escaping (AVCompositionTrack?, (any Error)?) -> Void
)
```

``` source
func loadTrack(withTrackID trackID: CMPersistentTrackID) async throws -> AVCompositionTrack?
```

## Parameters 

`trackID`  

The identifier of the track to load.

`completionHandler`  

A callback that the system invokes after it finishes the loading request. It passes the completion handler the following parameters:

track  
The loaded track, or `nil` if no track with the specified identifier exists or if an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## See Also

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVCompositionTrack]>

The tracks that a composition contains.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVCompositionTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVCompositionTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

