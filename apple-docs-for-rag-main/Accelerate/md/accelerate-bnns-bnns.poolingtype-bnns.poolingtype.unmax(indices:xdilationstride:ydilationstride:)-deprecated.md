

- Accelerate
- BNNS
- BNNS.PoolingType
-  BNNS.PoolingType.unMax(indices:xDilationStride:yDilationStride:) Deprecated

Case

# BNNS.PoolingType.unMax(indices:xDilationStride:yDilationStride:)

A function for pooling that’s the partial inverse of max pooling and sets all nonmaximal values to zero.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
case unMax(
    indices: UnsafeMutableBufferPointer? = nil,
    xDilationStride: Int = 0,
    yDilationStride: Int = 0
)
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Pooling Types

case average(countIncludesPadding: Bool)

A function for pooling that computes the average of each element in the pooling kernel.

Deprecated

case l2Norm

A function for pooling that computes the square root of the sum of squares of each element in the pooling kernel.

Deprecated

case max(indices: UnsafeMutableBufferPointer&lt;Int>?, xDilationStride: Int, yDilationStride: Int)

A function for pooling that computes the maximum of each element in the pooling kernel.

Deprecated

