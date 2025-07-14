

- Core ML
- MLTensor
-  transposed() 

Instance Method

# transposed()

Permutes the tensor with dimensions permuted in reverse order.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func transposed() -> MLTensor
```

## Return Value

A permuted tensor.

## Discussion

For example:

```
let x = MLTensor(shape: [1, 2, 3], scalars: [1, 2, 3, 4, 5, 6], scalarType: Float.self)
let y = x.transposed()
y.shape // is [3, 2, 1]
```

