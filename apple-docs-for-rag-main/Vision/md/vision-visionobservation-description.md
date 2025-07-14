

- Vision
- VisionObservation
-  description 

Instance Property

# description

A textual representation of this instance.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
override var description: String { get }
```

**Required**

## See Also

### Inspecting an observation

var uuid: UUID

A unique alphanumeric value that the framework assigns the observation.

**Required**

var confidence: Float

The level of confidence in the observation’s accuracy.

**Required**

var originatingRequestDescriptor: RequestDescriptor?

The descriptor of the request that produces the observation.

**Required**

enum RequestDescriptor

A type that describes the request and revision combination.

var timeRange: CMTimeRange?

The time range of the reported observation.

**Required**

