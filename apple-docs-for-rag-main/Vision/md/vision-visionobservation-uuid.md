

- Vision
- VisionObservation
-  uuid 

Instance Property

# uuid

A unique alphanumeric value that the framework assigns the observation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var uuid: UUID { get }
```

**Required**

## See Also

### Inspecting an observation

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

var timeRange: CMTimeRange?

The time range of the reported observation.

**Required**

