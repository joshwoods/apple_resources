

- Game Controller
- GCAxisInput
-  lastValueLatency 

Instance Property

# lastValueLatency

The time in seconds between the last value change and the current time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastValueLatency: TimeInterval { get }
```

**Required**

## Discussion

Use this property as a minimum latency value that may not include latency that accrues on the device or when it transmits the event.

## See Also

### Getting the value

var value: Float

The value along the axis, in unit coordinates.

**Required**

var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxisInput, Float) -> Void)?

The block that the input object calls when the value changes.

**Required**

var lastValueTimestamp: TimeInterval

The time of the most recent value change.

**Required**

