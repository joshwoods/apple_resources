

- AVFoundation
- AVVideoCompositionInstructionProtocol
-  requiredSourceSampleDataTrackIDs 

Instance Property

# requiredSourceSampleDataTrackIDs

The identifiers of the sample data tracks the instruction requires to compose frames.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
optional var requiredSourceSampleDataTrackIDs: [NSNumber] { get }
```

## Discussion

An empty array indicates the instruction requires no sample data.

## See Also

### Getting Track ID Settings

var passthroughTrackID: CMPersistentTrackID

An identifier of a source track to pass through without compositing.

**Required**

var requiredSourceTrackIDs: [NSValue]?

The identifiers of the video tracks the instruction requires to compose frames.

**Required**

