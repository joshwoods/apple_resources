

- Core ML
- MLTensor
-  init(randomUniform:in:seed:scalarType:) 

Initializer

# init(randomUniform:in:seed:scalarType:)

Creates a tensor with the specified shape, randomly sampling scalar values from a uniform distribution in `bounds`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    randomUniform shape: [Int],
    in bounds: Range = 0..

## Parameters 

`shape`  

The shape of the tensor.

`bounds`  

The bounds of the distribution. The default value is `0..

`seed`  

The random seed.

`scalarType`  

The scalar type.

## Discussion

Note

Using the same seed produces the same result only when dispatched to the same compute device.

