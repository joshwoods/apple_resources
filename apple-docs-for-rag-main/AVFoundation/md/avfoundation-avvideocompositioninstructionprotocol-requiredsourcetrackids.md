

- AVFoundation
- AVVideoCompositionInstructionProtocol
-  requiredSourceTrackIDs 

Instance Property

# requiredSourceTrackIDs

The identifiers of the video tracks the instruction requires to compose frames.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var requiredSourceTrackIDs: [NSValue]? { get }
```

**Required**

## Discussion

If the value of this property is `nil`, the instruction requires all source tracks for composition.

## See Also

### Getting Track ID Settings

var passthroughTrackID: CMPersistentTrackID

An identifier of a source track to pass through without compositing.

**Required**

var requiredSourceSampleDataTrackIDs: [NSNumber]

The identifiers of the sample data tracks the instruction requires to compose frames.

