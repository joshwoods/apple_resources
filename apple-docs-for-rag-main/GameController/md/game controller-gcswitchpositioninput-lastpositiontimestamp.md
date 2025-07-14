

- Game Controller
- GCSwitchPositionInput
-  lastPositionTimestamp 

Instance Property

# lastPositionTimestamp

A timestamp for when the profile reports the last position.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastPositionTimestamp: TimeInterval { get }
```

**Required**

## Discussion

This property isn’t a specific date and time. To determine the time between positions, subtract a previous value from the current value.

## See Also

### Getting the position

var position: Int

The position of the switch.

**Required**

var positionDidChangeHandler: ((any GCPhysicalInputElement, any GCSwitchPositionInput, Int) -> Void)?

The block that the profile calls when the value of the switch changes.

**Required**

var lastPositionLatency: TimeInterval

The time in seconds between the current and previous positions.

**Required**

