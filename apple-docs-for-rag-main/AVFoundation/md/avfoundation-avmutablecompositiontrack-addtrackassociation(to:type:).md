

- AVFoundation
- AVMutableCompositionTrack
-  addTrackAssociation(to:type:) 

Instance Method

# addTrackAssociation(to:type:)

Establishes a track association of a specific type between two tracks.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func addTrackAssociation(
    to compositionTrack: AVCompositionTrack,
    type trackAssociationType: AVAssetTrack.AssociationType
)
```

## Parameters 

`compositionTrack`  

A composition track to associate.

`trackAssociationType`  

The type of track association to create between tracks.

## See Also

### Associating Tracks

func removeTrackAssociation(to: AVCompositionTrack, type: AVAssetTrack.AssociationType)

Removes an association from a composition track.

