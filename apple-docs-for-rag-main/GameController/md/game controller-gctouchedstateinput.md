

- Game Controller
-  GCTouchedStateInput 

Protocol

# GCTouchedStateInput

The common properties for an element that has touch state input.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
protocol GCTouchedStateInput : NSObjectProtocol
```

## Topics

### Getting change information

var isTouched: Bool

A Boolean value that indicates whether the user touches the button.

**Required**

var lastTouchedStateTimestamp: TimeInterval

The time of the most recent touch state change.

**Required**

var lastTouchedStateLatency: TimeInterval

The time in seconds between the last touch state change and the current time.

**Required**

var touchedDidChangeHandler: ((any GCPhysicalInputElement, any GCTouchedStateInput, Bool) -> Void)?

A block that the element calls when its touch value changes.

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

protocol GCPressedStateInput

The common properties for an element that has press state input, such as input from a button.

