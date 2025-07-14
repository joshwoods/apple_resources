

- Game Controller
- GCAxis2DInput
-  value 

Instance Property

# value

The axis input represented as a normalized point in a two-dimensional coordinate system.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
var value: GCPoint2 { get }
```

**Required**

## Discussion

The values of the coordinates range between `-1` and `1` where `(0,0)` is the fixed origin. Game Controller deadzones and saturates the values so there’s no value outside this range. A zero coordinate is inside the deadzone and any coordinate greater than or less than zero is outside the deadzone.

## See Also

### Getting the value

struct GCPoint2

A structure that represents a normalized point in a two-dimensional coordinate system.

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxis2DInput, GCPoint2) -> Void)?

The block that the axis element calls when its value changes.

**Required**

var lastValueTimestamp: TimeInterval

The time of the most recent value change.

**Required**

var lastValueLatency: TimeInterval

The time in seconds between the last value change and the current time.

**Required**

