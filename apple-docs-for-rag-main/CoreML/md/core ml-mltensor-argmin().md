

- Core ML
- MLTensor
-  argmin() 

Instance Method

# argmin()

Returns the index of the minimum value of the flattened scalars.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func argmin() -> MLTensor
```

## Discussion

```
let x = MLTensor(shape: [3, 2], scalars: [2, 3, 4, 5, 6, 7], scalarType: Float.self)
let y = x.argmin()
y.shape // is []
y.scalarType // is Int32
await y.shapedArray(of: Int32.self) // is 0
```

