

- Core ML
- MLTensor
-  cast(like:) 

Instance Method

# cast(like:)

Casts the elements of the tensor to the scalar type of the given array.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func cast(like other: MLTensor) -> MLTensor
```

## Parameters 

`other`  

The other tensor whose scalar type is used for the cast.

## Return Value

A new tensor with its contents cast to the scalar type of `other`.

## Discussion

For example:

```
let x = MLTensor([1, 2, 3], scalarType: Float.self)
let y = MLTensor([1, 2, 3], scalarType: Int32.self)
let z = y.cast(like: x)
z.scalarType // is Float
```

