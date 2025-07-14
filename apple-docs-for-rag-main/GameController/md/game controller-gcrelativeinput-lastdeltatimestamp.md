

- Game Controller
- GCRelativeInput
-  lastDeltaTimestamp 

Instance Property

# lastDeltaTimestamp

A timestamp for when the profile reports the delta value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastDeltaTimestamp: TimeInterval { get }
```

**Required**

## Discussion

This property isn’t a specific date and time. To determine the time between delta values, subtract a previous value from the current value.

## See Also

### Getting the delta value and timestamp

var delta: Float

The most recent amount of change in values that the profile records.

**Required**

var deltaDidChangeHandler: ((any GCPhysicalInputElement, any GCRelativeInput, Float) -> Void)?

The block that the profile calls when the element’s input changes.

**Required**

var lastDeltaLatency: TimeInterval

The time in seconds between the current and the previous delta values.

**Required**

