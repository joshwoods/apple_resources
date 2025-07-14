

- AVFoundation
- AVAssetTrackGroup
-  trackIDs 

Instance Property

# trackIDs

The IDs of the tracks in the group.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var trackIDs: [NSNumber] { get }
```

## Discussion

The value of this property is an array of NSNumber instances used as CMPersistentTrackID values, one for each track in the group.

