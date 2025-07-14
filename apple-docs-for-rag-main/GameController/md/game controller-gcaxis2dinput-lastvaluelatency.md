

- Game Controller
- GCAxis2DInput
-  lastValueLatency 

Instance Property

# lastValueLatency

The time in seconds between the last value change and the current time.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
var lastValueLatency: TimeInterval { get }
```

**Required**

## Discussion

Use this property as a minimum latency value that may not include latency that accrues on the device or when it transmits the event.

## See Also

### Getting the value

var value: GCPoint2

The axis input represented as a normalized point in a two-dimensional coordinate system.

**Required**

struct GCPoint2

A structure that represents a normalized point in a two-dimensional coordinate system.

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxis2DInput, GCPoint2) -> Void)?

The block that the axis element calls when its value changes.

**Required**

var lastValueTimestamp: TimeInterval

The time of the most recent value change.

**Required**

