

- Accelerate
-  BNNSPoolingFunctionUnMax 

Global Variable

# BNNSPoolingFunctionUnMax

A function for pooling that’s the partial inverse of max pooling and sets all nonmaximal values to zero.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSPoolingFunctionUnMax: BNNSPoolingFunction { get }
```

## See Also

### Raw Values

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSPoolingFunctionAverageCountIncludePadding: BNNSPoolingFunction

A function for pooling that computes the average of each element in the pooling kernel, including zero-padding.

var BNNSPoolingFunctionAverageCountExcludePadding: BNNSPoolingFunction

A function for pooling that computes the average of each element in the pooling kernel, excluding zero-padding.

var BNNSPoolingFunctionL2Norm: BNNSPoolingFunction

A function for pooling that computes the square root of the sum of squares of each element in the pooling kernel.

