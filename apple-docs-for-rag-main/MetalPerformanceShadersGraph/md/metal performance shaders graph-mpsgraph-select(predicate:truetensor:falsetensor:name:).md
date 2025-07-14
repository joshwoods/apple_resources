

- Metal Performance Shaders Graph
- MPSGraph
-  select(predicate:trueTensor:falseTensor:name:) 

Instance Method

# select(predicate:trueTensor:falseTensor:name:)

Selects values from either the true or false predicate tensor, depending on the values in the first input.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func select(
    predicate predicateTensor: MPSGraphTensor,
    trueTensor truePredicateTensor: MPSGraphTensor,
    falseTensor falseSelectTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`predicateTensor`  

The predicate tensor.

`truePredicateTensor`  

The tensor to select values from if predicate is true.

`falseSelectTensor`  

The tensor to select values from if predicate is false.

`name`  

An optional string which serves as an identifier for the operation.

## Return Value

A valid `MPSGraphTensor` object containing the elementwise result of the applied operation.

## Discussion

This operation creates a select operation and returns the result tensor. It supports broadcasting as well.

```
resultTensor = select(predicateTensor, truePredicateTensor, falseSelectTensor)
```

