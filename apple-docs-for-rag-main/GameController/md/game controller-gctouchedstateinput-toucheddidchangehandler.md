

- Game Controller
- GCTouchedStateInput
-  touchedDidChangeHandler 

Instance Property

# touchedDidChangeHandler

A block that the element calls when its touch value changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var touchedDidChangeHandler: ((any GCPhysicalInputElement, any GCTouchedStateInput, Bool) -> Void)? { get set }
```

**Required**

## Discussion

Use this property to get the latest state of the touch input. The block’s parameters are:

element  
The element whose value changes.

input  
The input of the element that changes.

touched  
A Boolean value that indicates whether the user touches the button.

## See Also

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

