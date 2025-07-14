

- Game Controller
- GCTouchedStateInput
-  lastTouchedStateTimestamp 

Instance Property

# lastTouchedStateTimestamp

The time of the most recent touch state change.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastTouchedStateTimestamp: TimeInterval { get }
```

**Required**

## Discussion

This property isn’t a specific date and time. To determine the time between changes, subtract a previous value from the current value.

## See Also

### Getting change information

var isTouched: Bool

A Boolean value that indicates whether the user touches the button.

**Required**

var lastTouchedStateLatency: TimeInterval

The time in seconds between the last touch state change and the current time.

**Required**

var touchedDidChangeHandler: ((any GCPhysicalInputElement, any GCTouchedStateInput, Bool) -> Void)?

A block that the element calls when its touch value changes.

**Required**

