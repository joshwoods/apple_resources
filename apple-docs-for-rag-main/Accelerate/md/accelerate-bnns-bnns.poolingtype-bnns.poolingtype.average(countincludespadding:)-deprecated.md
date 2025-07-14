

- Accelerate
- BNNS
- BNNS.PoolingType
-  BNNS.PoolingType.average(countIncludesPadding:) Deprecated

Case

# BNNS.PoolingType.average(countIncludesPadding:)

A function for pooling that computes the average of each element in the pooling kernel.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case average(countIncludesPadding: Bool)
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Pooling Types

case l2Norm

A function for pooling that computes the square root of the sum of squares of each element in the pooling kernel.

Deprecated

case max(indices: UnsafeMutableBufferPointer&lt;Int>?, xDilationStride: Int, yDilationStride: Int)

A function for pooling that computes the maximum of each element in the pooling kernel.

Deprecated

case unMax(indices: UnsafeMutableBufferPointer&lt;Int>?, xDilationStride: Int, yDilationStride: Int)

A function for pooling that’s the partial inverse of max pooling and sets all nonmaximal values to zero.

Deprecated

