

- AVFoundation
- AVMutableMovie
-  loadTrack(withTrackID:completionHandler:) 

Instance Method

# loadTrack(withTrackID:completionHandler:)

Loads a track that contains the specified identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
func loadTrack(
    withTrackID trackID: CMPersistentTrackID,
    completionHandler: @escaping (AVMutableMovieTrack?, (any Error)?) -> Void
)
```

``` source
func loadTrack(withTrackID trackID: CMPersistentTrackID) async throws -> AVMutableMovieTrack?
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

static var tracks: AVAsyncProperty&lt;Root, [AVMutableMovieTrack]>

The tracks that a movie contains.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVMutableMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVMutableMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

