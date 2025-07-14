

- Game Controller
- GCPressedStateInput
-  isPressed 

Instance Property

# isPressed

A Boolean value that indicates whether the user presses the button.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var isPressed: Bool { get }
```

**Required**

## See Also

### Getting change information

var lastPressedStateTimestamp: TimeInterval

The time of the most recent press state change.

**Required**

var lastPressedStateLatency: TimeInterval

The time in seconds between the last press state change and the current time.

**Required**

var pressedDidChangeHandler: ((any GCPhysicalInputElement, any GCPressedStateInput, Bool) -> Void)?

The block that the profile calls when an element’s press state changes.

**Required**

