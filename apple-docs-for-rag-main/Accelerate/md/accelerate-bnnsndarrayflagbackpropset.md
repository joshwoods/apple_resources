

- Accelerate
-  BNNSNDArrayFlagBackpropSet 

Global Variable

# BNNSNDArrayFlagBackpropSet

A flag that indicates the elements of this n-dimensional array are overwritten by the Jacobian during backpropagation.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSNDArrayFlagBackpropSet: BNNSNDArrayFlags { get }
```

## See Also

### N-Dimensional Array Flags

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSNDArrayFlagBackpropAccumulate: BNNSNDArrayFlags

A flag that indicates backpropagation adds the value of the Jacobian to the elements of this n-dimensional array.

