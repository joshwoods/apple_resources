

- AVFoundation
- AVPartialAsyncProperty
-  availableTrackAssociationTypes 

Type Property

# availableTrackAssociationTypes

An array of association types that the track uses to associate with other tracks.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var availableTrackAssociationTypes: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Track Associations

func loadAssociatedTracks(ofType: AVAssetTrack.AssociationType, completionHandler: ([AVAssetTrack]?, (any Error)?) -> Void)

Loads associated tracks that have the specified association type.

