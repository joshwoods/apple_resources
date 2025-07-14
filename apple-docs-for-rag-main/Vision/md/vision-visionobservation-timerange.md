

- Vision
- VisionObservation
-  timeRange 

Instance Property

# timeRange

The time range of the reported observation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var timeRange: CMTimeRange? { get }
```

**Required**

## Discussion

When evaluating a sequence of image buffers, use this property to determine each observation’s start time and duration. If a request doesn’t support time ranges, or the time range is unknown, the value of this property is `nil`.

## See Also

### Inspecting an observation

var uuid: UUID

A unique alphanumeric value that the framework assigns the observation.

**Required**

var confidence: Float

The level of confidence in the observation’s accuracy.

**Required**

var description: String

A textual representation of this instance.

**Required**

var originatingRequestDescriptor: RequestDescriptor?

The descriptor of the request that produces the observation.

**Required**

enum RequestDescriptor

A type that describes the request and revision combination.

