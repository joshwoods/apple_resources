

- Accelerate
- BNNS
-  BNNS.ReductionFunction 

Enumeration

# BNNS.ReductionFunction

Constants that describe reduction functions.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum ReductionFunction
```

## Topics

### Reduction Functions

case max

A reduction function that computes the maximum value.

case argMax

A reduction function that computes the index of the maximum value.

case mean

A function for reduction that computes the mean value.

case meanNonZero

A reduction function that computes the mean value of nonzero elements.

case min

A reduction function that computes the minimum value.

case argMin

A reduction function that computes the index of the minimum value.

case sum

A reduction function that computes the sum of all values.

case sumOfAbsolutes

A reduction function that computes the sum of all absolute values.

case sumOfLogs(epsilon: Float)

A reduction function that computes the sum of the natural logarithm of all values.

case sumOfSquares

A reduction function that computes the sum of the square of all values.

case logicalAnd

A reduction function that computes the logical AND of all values.

case all

An alias of the logical AND reduction function.

case logicalOr

A reduction function that computes the logical OR of all values.

case any

An alias of the logical OR reduction function.

### Instance Properties

var bnnsReduceFunction: BNNSReduceFunction

The underlying reduction function structure.

### Deprecated Symbols

case maxIndex

A function for reduction that computes the index of the maximum value.

Deprecated

case minIndex

A function for reduction that computes the index of the minimum value.

Deprecated

### Enumeration Cases

case l2Norm

case logSumExp

case product

