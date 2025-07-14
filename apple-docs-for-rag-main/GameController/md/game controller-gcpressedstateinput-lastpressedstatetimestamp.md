

- Game Controller
- GCPressedStateInput
-  lastPressedStateTimestamp 

Instance Property

# lastPressedStateTimestamp

The time of the most recent press state change.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastPressedStateTimestamp: TimeInterval { get }
```

**Required**

## Discussion

This property isn’t a specific date and time. To determine the time between changes, subtract a previous value from the current value.

## See Also

### Getting change information

var isPressed: Bool

A Boolean value that indicates whether the user presses the button.

**Required**

var lastPressedStateLatency: TimeInterval

The time in seconds between the last press state change and the current time.

**Required**

var pressedDidChangeHandler: ((any GCPhysicalInputElement, any GCPressedStateInput, Bool) -> Void)?

The block that the profile calls when an element’s press state changes.

**Required**

