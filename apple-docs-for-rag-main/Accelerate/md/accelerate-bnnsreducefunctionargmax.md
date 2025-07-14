

- Accelerate
-  BNNSReduceFunctionArgMax 

Global Variable

# BNNSReduceFunctionArgMax

A reduction function that computes the index of the maximum value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSReduceFunctionArgMax: BNNSReduceFunction { get }
```

## See Also

### Reduction Functions

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

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

var BNNSReduceFunctionSum: BNNSReduceFunction

A reduction function that computes the sum of all values.

