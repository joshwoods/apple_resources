

- Core ML
- MLTensor
-  squeezingShape() 

Instance Method

# squeezingShape()

Removes all dimensions of size 1 from the shape of the tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func squeezingShape() -> MLTensor
```

## Discussion

For example:

```
let x = MLTensor(shape: [1, 2, 1], scalars: [1, 2], scalarType: Float.self)
let y = x.squeezingShape()
y.shape // is [2]
```

