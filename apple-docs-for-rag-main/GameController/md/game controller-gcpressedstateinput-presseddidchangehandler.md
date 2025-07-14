

- Game Controller
- GCPressedStateInput
-  pressedDidChangeHandler 

Instance Property

# pressedDidChangeHandler

The block that the profile calls when an element’s press state changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var pressedDidChangeHandler: ((any GCPhysicalInputElement, any GCPressedStateInput, Bool) -> Void)? { get set }
```

**Required**

## Mentioned in 

Handling input events

## Discussion

The block’s parameters are:

`element`  
The element whose value changed.

`input`  
The press state of the element.

## See Also

### Getting change information

var isPressed: Bool

A Boolean value that indicates whether the user presses the button.

**Required**

var lastPressedStateTimestamp: TimeInterval

The time of the most recent press state change.

**Required**

var lastPressedStateLatency: TimeInterval

The time in seconds between the last press state change and the current time.

**Required**

