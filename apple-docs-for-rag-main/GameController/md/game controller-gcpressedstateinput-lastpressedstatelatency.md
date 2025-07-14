

- Game Controller
- GCPressedStateInput
-  lastPressedStateLatency 

Instance Property

# lastPressedStateLatency

The time in seconds between the last press state change and the current time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastPressedStateLatency: TimeInterval { get }
```

**Required**

## Discussion

Use this property as a minimum latency value that may not include latency that accrues on the device or when it transmits the event.

## See Also

### Getting change information

var isPressed: Bool

A Boolean value that indicates whether the user presses the button.

**Required**

var lastPressedStateTimestamp: TimeInterval

The time of the most recent press state change.

**Required**

var pressedDidChangeHandler: ((any GCPhysicalInputElement, any GCPressedStateInput, Bool) -> Void)?

The block that the profile calls when an element’s press state changes.

**Required**

