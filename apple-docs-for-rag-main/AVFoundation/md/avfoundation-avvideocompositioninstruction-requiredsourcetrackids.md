

- AVFoundation
- AVVideoCompositionInstruction
-  requiredSourceTrackIDs 

Instance Property

# requiredSourceTrackIDs

The identifiers of source video tracks that the compositor requires to compose frames for the instruction.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var requiredSourceTrackIDs: [NSValue] { get }
```

## See Also

### Identifying Source Tracks

var requiredSourceSampleDataTrackIDs: [NSNumber]

The identifiers of source sample data tracks that the compositor requires to compose frames for the instruction.

var passthroughTrackID: CMPersistentTrackID

The track identifier from an instruction source frame.

