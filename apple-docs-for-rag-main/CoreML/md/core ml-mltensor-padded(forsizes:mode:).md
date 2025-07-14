

- Core ML
- MLTensor
-  padded(forSizes:mode:) 

Instance Method

# padded(forSizes:mode:)

Returns a padded tensor according to the specified padding sizes and mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func padded(
    forSizes sizes: [(before: Int, after: Int)],
    mode: MLTensor.PaddingMode
) -> MLTensor
```

## Parameters 

`sizes`  

An array of tuples describing the size to be inserted before and after each dimension.

`mode`  

The mode of padding, etiher constant, reflection, or symmetric.

## Return Value

The padded tensor.

## Discussion

For example:

```
let x = MLTensor(shape: [2, 3], scalars: [
    1, 2, 3,
    4, 5, 6
], scalarType: Float32.self)

let constantPadding = x.padded(forSizes: [(0, 0), (2, 2)], mode: .constant(Float(0)))
// [[0, 0, 1, 2, 3, 0, 0],
//  [0, 0, 4, 5, 6, 0, 0]]

let reflectionPadding = x.padded(forSizes: [(0, 0), (2, 2)], mode: .reflection)
// [[3, 2, 1, 2, 3, 2, 1],
//  [6, 5, 4, 5, 6, 5, 4]]

let symmetricPadding = x.padded(forSizes: [(0, 0), (2, 2)], mode: .symmetric)
// [[2, 1, 1, 2, 3, 3, 2],
//  [5, 4, 4, 5, 6, 6, 5]]
```

