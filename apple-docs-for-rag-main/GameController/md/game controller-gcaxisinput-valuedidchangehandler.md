

- Game Controller
- GCAxisInput
-  valueDidChangeHandler 

Instance Property

# valueDidChangeHandler

The block that the input object calls when the value changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var valueDidChangeHandler: ((any GCPhysicalInputElement, any GCAxisInput, Float) -> Void)? { get set }
```

**Required**

## Discussion

The block’s parameters are:

`element`  
The element whose value changed.

`input`  
The input object that changed.

`value`  
The value of the axis at the time the input object calls this handler.

## See Also

### Getting the value

var value: Float

The value along the axis, in unit coordinates.

**Required**

var lastValueTimestamp: TimeInterval

The time of the most recent value change.

**Required**

var lastValueLatency: TimeInterval

The time in seconds between the last value change and the current time.

**Required**

