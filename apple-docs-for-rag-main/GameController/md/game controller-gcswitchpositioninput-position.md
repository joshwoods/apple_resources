

- Game Controller
- GCSwitchPositionInput
-  position 

Instance Property

# position

The position of the switch.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var position: Int { get }
```

**Required**

## See Also

### Getting the position

var positionDidChangeHandler: ((any GCPhysicalInputElement, any GCSwitchPositionInput, Int) -> Void)?

The block that the profile calls when the value of the switch changes.

**Required**

var lastPositionTimestamp: TimeInterval

A timestamp for when the profile reports the last position.

**Required**

var lastPositionLatency: TimeInterval

The time in seconds between the current and previous positions.

**Required**

