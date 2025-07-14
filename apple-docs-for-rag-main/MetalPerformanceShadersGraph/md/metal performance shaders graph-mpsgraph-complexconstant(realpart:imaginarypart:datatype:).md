

- Metal Performance Shaders Graph
- MPSGraph
-  complexConstant(realPart:imaginaryPart:dataType:) 

Instance Method

# complexConstant(realPart:imaginaryPart:dataType:)

Creates a complex constant operation and returns the result tensor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func complexConstant(
    realPart: Double,
    imaginaryPart: Double,
    dataType: MPSDataType
) -> MPSGraphTensor
```

## Parameters 

`realPart`  

The real part of the complex scalar to fill the entire tensor values with.

`imaginaryPart`  

The imaginary part of the complex scalar to fill the entire tensor values with.

`dataType`  

The dataType of the constant tensor.

## Return Value

A valid MPSGraphTensor object.

