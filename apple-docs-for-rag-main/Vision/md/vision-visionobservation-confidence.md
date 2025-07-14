

- Vision
- VisionObservation
-  confidence 

Instance Property

# confidence

The level of confidence in the observation’s accuracy.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var confidence: Float { get }
```

**Required**

## Discussion

The Vision framework normalizes this value to `[0.0, 1.0]` under most circumstances. A value of `0.0` indicates no confidence. A value of `1.0` indicates highest confidence, or the observation doesn’t support or assign meaning to confidence.

## See Also

### Inspecting an observation

var uuid: UUID

A unique alphanumeric value that the framework assigns the observation.

**Required**

var description: String

A textual representation of this instance.

**Required**

var originatingRequestDescriptor: RequestDescriptor?

The descriptor of the request that produces the observation.

**Required**

enum RequestDescriptor

A type that describes the request and revision combination.

var timeRange: CMTimeRange?

The time range of the reported observation.

**Required**

