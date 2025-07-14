

- AVFoundation
- AVMutableVideoComposition
-  sourceTrackIDForFrameTiming 

Instance Property

# sourceTrackIDForFrameTiming

An identifier of the source track from which the video composition derives frame timing.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var sourceTrackIDForFrameTiming: CMPersistentTrackID { get set }
```

## Discussion

If an empty edit is encountered in the source asset’s track, the compositor composes frames as needed up to the frequency specified in frameDuration property. Otherwise the frame timing for the video composition is derived from the source asset’s track with the corresponding ID.

## See Also

### Identifying Source Tracks

var sourceSampleDataTrackIDs: [CMPersistentTrackID]

The identifiers of source sample data tracks in the composition that the object requires to compose frames.

