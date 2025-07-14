

- Game Controller
-  GCPressedStateInput 

Protocol

# GCPressedStateInput

The common properties for an element that has press state input, such as input from a button.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCPressedStateInput : NSObjectProtocol
```

## Topics

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

var pressedDidChangeHandler: ((any GCPhysicalInputElement, any GCPressedStateInput, Bool) -> Void)?

The block that the profile calls when an element’s press state changes.

**Required**

### Getting user actions

var sources: Set&lt;AnyHashable>

One or more physical actions the user performs to manipulate the input.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Button elements and names

protocol GCTouchedStateInput

The common properties for an element that has touch state input.

