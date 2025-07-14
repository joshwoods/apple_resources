

- AVFoundation
- AVFragmentedAsset
-  loadTracks(withMediaCharacteristic:completionHandler:) 

Instance Method

# loadTracks(withMediaCharacteristic:completionHandler:)

Loads tracks that contain media of a specified characteristic.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadTracks(
    withMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic,
    completionHandler: @escaping ([AVFragmentedAssetTrack]?, (any Error)?) -> Void
)
```

``` source
func loadTracks(withMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic) async throws -> [AVFragmentedAssetTrack]
```

## Parameters 

`mediaCharacteristic`  

The media characteristic of the tracks to load.

`completionHandler`  

A callback that the system invokes after it finishes the loading request. It passes the completion handler the following parameters:

tracks  
An array of tracks, which may be empty if no tracks with the specified media characteristic exist. The value is `nil` if an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## See Also

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVFragmentedAssetTrack]>

The tracks an asset contains.

func loadTrack(withTrackID: CMPersistentTrackID, completionHandler: (AVFragmentedAssetTrack?, (any Error)?) -> Void)

Loads a track that contains the specified identifier.

func loadTracks(withMediaType: AVMediaType, completionHandler: ([AVFragmentedAssetTrack]?, (any Error)?) -> Void)

Loads tracks that contain media of a specified type.

