

- Metal Performance Shaders Graph
- MPSGraphConvolution2DOpDescriptor
-  init(strideInX:strideInY:dilationRateInX:dilationRateInY:groups:paddingStyle:dataLayout:weightsLayout:) 

Initializer

# init(strideInX:strideInY:dilationRateInX:dilationRateInY:groups:paddingStyle:dataLayout:weightsLayout:)

Creates a convolution descriptor with given values for parameters.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
convenience init?(
    strideInX: Int,
    strideInY: Int,
    dilationRateInX: Int,
    dilationRateInY: Int,
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

`dilationRateInX`  

See dilationRateInX property.

`dilationRateInY`  

See dilationRateInY property.

`groups`  

See groups property.

`paddingStyle`  

See paddingStyle property.

`dataLayout`  

See dataLayout property.

`weightsLayout`  

See weightsLayout property.

## Return Value

The `MPSGraphConvolution2DOpDescriptor` on autoreleasepool.

