

- AVFoundation
- AVMutableMovieTrack
-  availableTrackAssociationTypes 

Instance Property

# availableTrackAssociationTypes

An array of association types that the track uses to associate with other tracks.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+watchOS 1.0+

``` source
var availableTrackAssociationTypes: [AVAssetTrack.AssociationType] { get }
```

## See Also

### Managing Track Associations

func associatedTracks(ofType: AVAssetTrack.AssociationType) -> [AVAssetTrack]

Returns an array of associated tracks that have the specified association type.

func addTrackAssociation(to: AVMovieTrack, type: AVAssetTrack.AssociationType)

Creates a specific type of track association between two tracks.

func removeTrackAssociation(to: AVMovieTrack, type: AVAssetTrack.AssociationType)

Removes a specific type of track association between two tracks.

