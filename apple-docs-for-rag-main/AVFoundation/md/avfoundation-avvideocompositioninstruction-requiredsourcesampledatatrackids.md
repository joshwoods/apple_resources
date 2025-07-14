

- AVFoundation
- AVVideoCompositionInstruction
-  requiredSourceSampleDataTrackIDs 

Instance Property

# requiredSourceSampleDataTrackIDs

The identifiers of source sample data tracks that the compositor requires to compose frames for the instruction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var requiredSourceSampleDataTrackIDs: [NSNumber] { get }
```

## See Also

### Identifying Source Tracks

var requiredSourceTrackIDs: [NSValue]

The identifiers of source video tracks that the compositor requires to compose frames for the instruction.

var passthroughTrackID: CMPersistentTrackID

The track identifier from an instruction source frame.

