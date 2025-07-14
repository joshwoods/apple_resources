

- Game Controller
- GCRelativeInput
-  lastDeltaLatency 

Instance Property

# lastDeltaLatency

The time in seconds between the current and the previous delta values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastDeltaLatency: TimeInterval { get }
```

**Required**

## Discussion

Use this property as a minimum latency value that may not include latency that accrues on the device or when it transmits the event.

## See Also

### Getting the delta value and timestamp

var delta: Float

The most recent amount of change in values that the profile records.

**Required**

var deltaDidChangeHandler: ((any GCPhysicalInputElement, any GCRelativeInput, Float) -> Void)?

The block that the profile calls when the element’s input changes.

**Required**

var lastDeltaTimestamp: TimeInterval

A timestamp for when the profile reports the delta value.

**Required**

