

- Metal Performance Shaders Graph
- MPSGraph
-  complexConstant(realPart:imaginaryPart:) 

Instance Method

# complexConstant(realPart:imaginaryPart:)

Creates a complex constant op with the MPSDataTypeComplexFloat32 data type and returns the result tensor.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func complexConstant(
    realPart: Double,
    imaginaryPart: Double
) -> MPSGraphTensor
```

## Parameters 

`realPart`  

The real part of the complex scalar to fill the entire tensor values with.

`imaginaryPart`  

The imaginary part of the complex scalar to fill the entire tensor values with.

## Return Value

A valid MPSGraphTensor object.

