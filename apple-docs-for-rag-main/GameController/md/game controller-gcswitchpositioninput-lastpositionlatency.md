

- Game Controller
- GCSwitchPositionInput
-  lastPositionLatency 

Instance Property

# lastPositionLatency

The time in seconds between the current and previous positions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastPositionLatency: TimeInterval { get }
```

**Required**

## Discussion

Use this property as a minimum latency value that may not include latency that accrues on the device or when it transmits the event.

## See Also

### Getting the position

var position: Int

The position of the switch.

**Required**

var positionDidChangeHandler: ((any GCPhysicalInputElement, any GCSwitchPositionInput, Int) -> Void)?

The block that the profile calls when the value of the switch changes.

**Required**

var lastPositionTimestamp: TimeInterval

A timestamp for when the profile reports the last position.

**Required**

