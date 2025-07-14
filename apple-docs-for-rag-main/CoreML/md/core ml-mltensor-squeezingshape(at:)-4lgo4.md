

- Core ML
- MLTensor
-  squeezingShape(at:) 

Instance Method

# squeezingShape(at:)

Removes the specified dimensions of size 1 from the shape of the tensor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func squeezingShape(at axes: Int...) -> MLTensor
```

## Parameters 

`axes`  

The axes to remove if the size is `1`.

## Discussion

For example:

```
let x = MLTensor(shape: [1, 2, 1], scalars: [1, 2], scalarType: Float.self)
let y = x.squeezingShape(at: 0)
y.shape // is [2, 1]
```

