

- Game Controller
- GCTouchedStateInput
-  lastTouchedStateLatency 

Instance Property

# lastTouchedStateLatency

The time in seconds between the last touch state change and the current time.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var lastTouchedStateLatency: TimeInterval { get }
```

**Required**

## Discussion

Use this property as a minimum latency value that may not include latency that accrues on the device or when it transmits the event.

## See Also

### Getting change information

var isTouched: Bool

A Boolean value that indicates whether the user touches the button.

**Required**

var lastTouchedStateTimestamp: TimeInterval

The time of the most recent touch state change.

**Required**

var touchedDidChangeHandler: ((any GCPhysicalInputElement, any GCTouchedStateInput, Bool) -> Void)?

A block that the element calls when its touch value changes.

**Required**

