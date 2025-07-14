

- AVFoundation
- AVVideoComposition
-  sourceSampleDataTrackIDs 

Instance Property

# sourceSampleDataTrackIDs

The identifiers of source sample data tracks in the composition that the object requires to compose frames.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@objc(_sourceSampleDataTrackIDs)
dynamic var sourceSampleDataTrackIDs: [CMPersistentTrackID] { get }
```

## See Also

### Identifying Source Tracks

var sourceTrackIDForFrameTiming: CMPersistentTrackID

An identifier of the source track from which the video composition derives frame timing.

