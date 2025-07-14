

- Core ML
- MLTensor
-  cast(to:) 

Instance Method

# cast(to:)

Casts the elements of the tensor to the given scalar type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func cast(to scalarType: Scalar.Type) -> MLTensor where Scalar : MLTensorScalar
```

## Parameters 

`scalarType`  

The destination scalar type.

## Return Value

A new tensor with its contents cast to the given scalar type.

## Discussion

For example:

```
let x = MLTensor([1, 2, 3], scalarType: Int32.self)
let y = x.cast(to: Float.self)
y.scalarType // is Float
```

