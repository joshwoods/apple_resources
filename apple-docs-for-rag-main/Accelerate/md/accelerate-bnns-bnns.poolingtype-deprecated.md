

- Accelerate
- BNNS
-  BNNS.PoolingType Deprecated

Enumeration

# BNNS.PoolingType

Constants that describe pooling types.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
enum PoolingType
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Pooling Types

case average(countIncludesPadding: Bool)

A function for pooling that computes the average of each element in the pooling kernel.

case l2Norm

A function for pooling that computes the square root of the sum of squares of each element in the pooling kernel.

case max(indices: UnsafeMutableBufferPointer&lt;Int>?, xDilationStride: Int, yDilationStride: Int)

A function for pooling that computes the maximum of each element in the pooling kernel.

case unMax(indices: UnsafeMutableBufferPointer&lt;Int>?, xDilationStride: Int, yDilationStride: Int)

A function for pooling that’s the partial inverse of max pooling and sets all nonmaximal values to zero.

### Instance Properties

var bnnsPoolingFunction: BNNSPoolingFunction

The underlying pooling function structure.

### Enumeration Cases

case maxEx(indicesDescriptor: BNNSNDArrayDescriptor?, xDilationStride: Int, yDilationStride: Int)

case unMaxEx(indicesDescriptor: BNNSNDArrayDescriptor, xDilationStride: Int, yDilationStride: Int)

