

- AVFoundation
- AVMutableCompositionTrack
-  removeTrackAssociation(to:type:) 

Instance Method

# removeTrackAssociation(to:type:)

Removes an association from a composition track.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func removeTrackAssociation(
    to compositionTrack: AVCompositionTrack,
    type trackAssociationType: AVAssetTrack.AssociationType
)
```

## Parameters 

`compositionTrack`  

A composition track to remove the association from.

`trackAssociationType`  

The type of track association to remove.

## See Also

### Associating Tracks

func addTrackAssociation(to: AVCompositionTrack, type: AVAssetTrack.AssociationType)

Establishes a track association of a specific type between two tracks.

