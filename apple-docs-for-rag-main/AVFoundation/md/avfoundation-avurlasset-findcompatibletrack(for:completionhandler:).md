

- AVFoundation
- AVURLAsset
-  findCompatibleTrack(for:completionHandler:) 

Instance Method

# findCompatibleTrack(for:completionHandler:)

Loads an asset track from which you can insert any time range into the composition track.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func findCompatibleTrack(
    for compositionTrack: AVCompositionTrack,
    completionHandler: @escaping (AVAssetTrack?, (any Error)?) -> Void
)
```

``` source
func findCompatibleTrack(for compositionTrack: AVCompositionTrack) async throws -> AVAssetTrack?
```

## Parameters 

`compositionTrack`  

A composition track to request an asset track for.

`completionHandler`  

A callback the system invokes after it finishes the request. The system calls the completion handler with the following arguments:

track  
The compatible asset track, or `nil` if there isn’t one or an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## Discussion

This method is the logical complement of mutableTrack(compatibleWith:).

## See Also

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVAssetTrack]>

The tracks an asset contains.

