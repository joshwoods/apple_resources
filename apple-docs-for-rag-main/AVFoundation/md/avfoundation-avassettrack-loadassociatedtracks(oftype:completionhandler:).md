

- AVFoundation
- AVAssetTrack
-  loadAssociatedTracks(ofType:completionHandler:) 

Instance Method

# loadAssociatedTracks(ofType:completionHandler:)

Loads associated tracks that have the specified association type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func loadAssociatedTracks(
    ofType trackAssociationType: AVAssetTrack.AssociationType,
    completionHandler: @escaping ([AVAssetTrack]?, (any Error)?) -> Void
)
```

``` source
func loadAssociatedTracks(ofType trackAssociationType: AVAssetTrack.AssociationType) async throws -> [AVAssetTrack]
```

## Parameters 

`trackAssociationType`  

The track association type to load tracks for.

`completionHandler`  

A callback that the system invokes after it finishes the loading request. It passes the completion handler the following parameters:

tracks  
The array of associated tracks, which may be empty if there are no tracks for the specified association type. The value is `nil` if an error occurs.

error  
An error object if the request fails; otherwise, `nil`.

## See Also

### Loading Track Associations

static var availableTrackAssociationTypes: AVAsyncProperty&lt;Root, [AVAssetTrack.AssociationType]>

An array of association types that the track uses to associate with other tracks.

