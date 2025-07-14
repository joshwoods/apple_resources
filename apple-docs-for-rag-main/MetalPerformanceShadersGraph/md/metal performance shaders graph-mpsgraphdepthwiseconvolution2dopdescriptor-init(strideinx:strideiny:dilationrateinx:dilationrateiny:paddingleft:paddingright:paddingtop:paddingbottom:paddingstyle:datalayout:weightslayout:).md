

- Metal Performance Shaders Graph
- MPSGraphDepthwiseConvolution2DOpDescriptor
-  init(strideInX:strideInY:dilationRateInX:dilationRateInY:paddingLeft:paddingRight:paddingTop:paddingBottom:paddingStyle:dataLayout:weightsLayout:) 

Initializer

# init(strideInX:strideInY:dilationRateInX:dilationRateInY:paddingLeft:paddingRight:paddingTop:paddingBottom:paddingStyle:dataLayout:weightsLayout:)

Creates a 2D-depthwise convolution descriptor with given values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
convenience init?(
    strideInX: Int,
    strideInY: Int,
    dilationRateInX: Int,
    dilationRateInY: Int,
    paddingLeft: Int,
    paddingRight: Int,
    paddingTop: Int,
    paddingBottom: Int,
    paddingStyle: MPSGraphPaddingStyle,
    dataLayout: MPSGraphTensorNamedDataLayout,
    weightsLayout: MPSGraphTensorNamedDataLayout
)
```

## Parameters 

`strideInX`  

See `strideInX` property.

`strideInY`  

See `strideInY` property.

`dilationRateInX`  

See `dilationRateInX` property.

`dilationRateInY`  

See `dilationRateInY` property.

`paddingLeft`  

See `paddingLeft` property.

`paddingRight`  

See `paddingRight` property.

`paddingTop`  

See `paddingTop` property.

`paddingBottom`  

See `paddingBottom` property.

`paddingStyle`  

See `paddingStyle` property.

`dataLayout`  

See `dataLayout` property.

`weightsLayout`  

See `weightsLayout` property.

## Return Value

The descriptor on autoreleasepool.

