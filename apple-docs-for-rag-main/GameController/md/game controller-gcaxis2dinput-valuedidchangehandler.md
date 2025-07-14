

- Game Controller
- GCAxis2DInput
-  valueDidChangeHandler 

Instance Property

# valueDidChangeHandler

The block that the axis element calls when its value changes.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxis2DInput, GCPoint2) -> Void)? { get set }
```

**Required**

## Discussion

The block’s parameters are:

`element`  
The element with the value that changes.

`input`  
The input on the element that changes.

`value`  
The value of the input when the element invokes this handler.

## See Also

### Getting the value

var value: GCPoint2

The axis input represented as a normalized point in a two-dimensional coordinate system.

**Required**

struct GCPoint2

A structure that represents a normalized point in a two-dimensional coordinate system.

var lastValueTimestamp: TimeInterval

The time of the most recent value change.

**Required**

var lastValueLatency: TimeInterval

The time in seconds between the last value change and the current time.

**Required**

