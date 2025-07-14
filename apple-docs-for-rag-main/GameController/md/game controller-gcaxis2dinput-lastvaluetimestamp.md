

- Game Controller
- GCAxis2DInput
-  lastValueTimestamp 

Instance Property

# lastValueTimestamp

The time of the most recent value change.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
var lastValueTimestamp: TimeInterval { get }
```

**Required**

## Discussion

This property isn’t a specific date and time. To determine the time between value changes in seconds, subtract a previous time from the current time.

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

var lastValueLatency: TimeInterval

The time in seconds between the last value change and the current time.

**Required**

