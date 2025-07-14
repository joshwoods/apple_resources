

- Game Controller
- GCPhysicalInputProfile
-  valueDidChangeHandler 

Instance Property

# valueDidChangeHandler

The block that the profile calls when an element’s value changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var valueDidChangeHandler: ((GCPhysicalInputProfile, GCControllerElement) -> Void)? { get set }
```

## Discussion

The block’s parameters are:

`profile`  
The controller profile that contains the element.

`element`  
The element with the value that changes.

If multiple elements change values at the same time, the profile calls this block once for each element that changes. If the value of a subelement changes, the profile only calls the block for the containing element.

## See Also

### Getting change information

var lastEventTimestamp: TimeInterval

The time of the most recent change to an element’s value.

