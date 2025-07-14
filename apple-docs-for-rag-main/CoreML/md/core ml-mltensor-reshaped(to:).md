

- Core ML
- MLTensor
-  reshaped(to:) 

Instance Method

# reshaped(to:)

Reshape to the specified shape.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func reshaped(to newShape: [Int]) -> MLTensor
```

## Parameters 

`newShape`  

The new shape of the array. The number of scalars matches the new shape.

## Discussion

For example:

```
let x = MLTensor(shape: [2], scalars: [1, 2], scalarType: Float.self)
let y = x.reshaped(at: [1, 2, 1])
y.shape // is [1, 2, 1]
```

