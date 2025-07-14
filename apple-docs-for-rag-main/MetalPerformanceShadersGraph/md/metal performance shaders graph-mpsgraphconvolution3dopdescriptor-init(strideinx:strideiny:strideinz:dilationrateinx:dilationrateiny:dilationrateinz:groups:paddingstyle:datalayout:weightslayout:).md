

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  init(strideInX:strideInY:strideInZ:dilationRateInX:dilationRateInY:dilationRateInZ:groups:paddingStyle:dataLayout:weightsLayout:) 

Initializer

# init(strideInX:strideInY:strideInZ:dilationRateInX:dilationRateInY:dilationRateInZ:groups:paddingStyle:dataLayout:weightsLayout:)

Creates a convolution descriptor with given values for parameters.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
convenience init?(
    strideInX: Int,
    strideInY: Int,
    strideInZ: Int,
    dilationRateInX: Int,
    dilationRateInY: Int,
    dilationRateInZ: Int,
    groups: Int,
    paddingStyle: MPSGraphPaddingStyle,
    dataLayout: MPSGraphTensorNamedDataLayout,
    weightsLayout: MPSGraphTensorNamedDataLayout
)
```

## Parameters 

`strideInX`  

See strideInX property.

`strideInY`  

See strideInY property.

`strideInZ`  

See strideInZ property.

`dilationRateInX`  

See dilationRateInX property.

`dilationRateInY`  

See dilationRateInY property.

`dilationRateInZ`  

See dilationRateInZ property.

`groups`  

See groups property.

`paddingStyle`  

See paddingStyle property.

`dataLayout`  

See dataLayout property.

`weightsLayout`  

See weightsLayout property.

## Return Value

The `MPSGraphConvolution3DOpDescriptor` on autoreleasepool.

