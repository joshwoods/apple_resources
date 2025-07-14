

- AVFoundation
- AVMutableMovieTrack
-  removeTrackAssociation(to:type:) 

Instance Method

# removeTrackAssociation(to:type:)

Removes a specific type of track association between two tracks.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func removeTrackAssociation(
    to movieTrack: AVMovieTrack,
    type trackAssociationType: AVAssetTrack.AssociationType
)
```

## Parameters 

`movieTrack`  

The AVMovieTrack object that is associated with the receiver.

`trackAssociationType`  

The type of track association to remove between the receiver and the specified movie track.

## See Also

### Managing Track Associations

var availableTrackAssociationTypes: [AVAssetTrack.AssociationType]

An array of association types that the track uses to associate with other tracks.

func associatedTracks(ofType: AVAssetTrack.AssociationType) -> [AVAssetTrack]

Returns an array of associated tracks that have the specified association type.

func addTrackAssociation(to: AVMovieTrack, type: AVAssetTrack.AssociationType)

Creates a specific type of track association between two tracks.

