

- Core ML
- MLTensor
-  rank 

Instance Property

# rank

The number of dimensions of the tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var rank: Int { get }
```

## Discussion

Rank is equal to the number of dimensions of the shape, i.e., `tensor.rank == tensor.shape.count`.

