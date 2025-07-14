

- AVFoundation
- AVFragmentedMovie
-  loadTracks(withMediaType:completionHandler:) 

Instance Method

# loadTracks(withMediaType:completionHandler:)

Loads tracks that contain media of a specified type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 8.0+

``` source
func loadTracks(
    withMediaType mediaType: AVMediaType,
    completionHandler: @escaping ([AVFragmentedMovieTrack]?, (any Error)?) -> Void
)
```

``` source
func loadTracks(withMediaType mediaType: AVMediaType) async throws -> [AVFragmentedMovieTrack]
```

## Parameters 

`mediaType`  

The media type of the tracks to load.

`completionHandler`  

A callback that the system invokes after it finishes the loading operation. It passes the completion handler the following parameters:

tracks  
An array of tracks, which may be empty if no tracks with the specified media type exist. The value is `nil` if an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## See Also

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVFragmentedMovieTrack]>

The tracks that a movie contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVFragmentedMovieTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVFragmentedMovieTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

