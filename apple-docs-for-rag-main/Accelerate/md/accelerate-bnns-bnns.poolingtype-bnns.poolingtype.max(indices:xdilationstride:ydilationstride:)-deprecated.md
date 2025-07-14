

- Accelerate
- BNNS
- BNNS.PoolingType
-  BNNS.PoolingType.max(indices:xDilationStride:yDilationStride:) Deprecated

Case

# BNNS.PoolingType.max(indices:xDilationStride:yDilationStride:)

A function for pooling that computes the maximum of each element in the pooling kernel.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

``` source
case max(
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

case unMax(indices: UnsafeMutableBufferPointer&lt;Int>?, xDilationStride: Int, yDilationStride: Int)

A function for pooling that’s the partial inverse of max pooling and sets all nonmaximal values to zero.

Deprecated

