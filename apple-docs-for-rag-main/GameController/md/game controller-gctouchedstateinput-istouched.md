

- Game Controller
- GCTouchedStateInput
-  isTouched 

Instance Property

# isTouched

A Boolean value that indicates whether the user touches the button.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var isTouched: Bool { get }
```

**Required**

## Discussion

For controllers that support capacitive touch, the user can start touching the button without pressure when the value property is `0`. For controllers that don’t support capacitive touch, the user starts touching the button when the value property is greater than `0`.

## See Also

### Getting change information

var lastTouchedStateTimestamp: TimeInterval

The time of the most recent touch state change.

**Required**

var lastTouchedStateLatency: TimeInterval

The time in seconds between the last touch state change and the current time.

**Required**

var touchedDidChangeHandler: ((any GCPhysicalInputElement, any GCTouchedStateInput, Bool) -> Void)?

A block that the element calls when its touch value changes.

**Required**

