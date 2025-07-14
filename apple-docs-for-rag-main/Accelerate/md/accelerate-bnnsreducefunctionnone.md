

- Accelerate
-  BNNSReduceFunctionNone 

Global Variable

# BNNSReduceFunctionNone

A reduction function that copies the input to the output.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var BNNSReduceFunctionNone: BNNSReduceFunction { get }
```

## Discussion

BNNS provides this reduction function for use with some functions — such as BNNSScatter(_:_:_:_:_:_:) — to indicate that the operation copies the input to the output. BNNSReduceFunctionNone isn’t supported by the BNNS reduction layer, use BNNSCopy(_:_:_:) to perform a copy or conversion operation.

## See Also

### Reduction Functions

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSReduceFunctionArgMax: BNNSReduceFunction

A reduction function that computes the index of the maximum value.

var BNNSReduceFunctionArgMin: BNNSReduceFunction

A reduction function that computes the index of the minimum value.

var BNNSReduceFunctionL1Norm: BNNSReduceFunction

A reduction function that computes the sum of the absolute value of each element.

var BNNSReduceFunctionLogicalAnd: BNNSReduceFunction

A reduction function that reduces a tensor to true if all elements are true.

var BNNSReduceFunctionAll: BNNSReduceFunction

An alias of the logical AND reduction function.

var BNNSReduceFunctionLogicalOr: BNNSReduceFunction

A reduction function that reduces a tensor to true if any element is true.

var BNNSReduceFunctionLogSum: BNNSReduceFunction

var BNNSReduceFunctionAny: BNNSReduceFunction

An alias of the logical OR reduction function.

var BNNSReduceFunctionMax: BNNSReduceFunction

A reduction function that computes the maximum value.

var BNNSReduceFunctionMean: BNNSReduceFunction

A reduction function that computes the mean value.

var BNNSReduceFunctionMeanNonZero: BNNSReduceFunction

A reduction function that computes the mean value of nonzero elements.

var BNNSReduceFunctionMin: BNNSReduceFunction

A reduction function that computes the minimum value.

