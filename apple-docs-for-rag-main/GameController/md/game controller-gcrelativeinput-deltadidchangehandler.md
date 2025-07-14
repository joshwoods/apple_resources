

- Game Controller
- GCRelativeInput
-  deltaDidChangeHandler 

Instance Property

# deltaDidChangeHandler

The block that the profile calls when the element’s input changes.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var deltaDidChangeHandler: ((any GCPhysicalInputElement, any GCRelativeInput, Float) -> Void)? { get set }
```

**Required**

## Discussion

The block’s parameters are:

`element`  
The element whose input changes.

`input`  
The input object that represents the relative or delta value.

`delta`  
The amount that the input changed since the last time the profile called this block.

## See Also

### Getting the delta value and timestamp

var delta: Float

The most recent amount of change in values that the profile records.

**Required**

var lastDeltaTimestamp: TimeInterval

A timestamp for when the profile reports the delta value.

**Required**

var lastDeltaLatency: TimeInterval

The time in seconds between the current and the previous delta values.

**Required**

