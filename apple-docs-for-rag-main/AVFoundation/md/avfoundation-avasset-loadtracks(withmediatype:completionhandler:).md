

- AVFoundation
- AVAsset
-  loadTracks(withMediaType:completionHandler:) 

Instance Method

# loadTracks(withMediaType:completionHandler:)

Loads tracks that contain media of a specified type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadTracks(
    withMediaType mediaType: AVMediaType,
    completionHandler: @escaping ([AVAssetTrack]?, (any Error)?) -> Void
)
```

``` source
func loadTracks(withMediaType mediaType: AVMediaType) async throws -> [AVAssetTrack]
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

## Mentioned in 

Loading media data asynchronously

## See Also

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVAssetTrack]>

The tracks of media that an asset contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVAssetTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaCharacteristic: AVMediaCharacteristic, completionHandler: ([AVAssetTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified characteristic.

func findUnusedTrackID(completionHandler: (CMPersistentTrackID, (any Error)?) -> Void)

Loads an identifier that no other track in the asset uses.

