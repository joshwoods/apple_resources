

- Metal Performance Shaders Graph
- MPSGraphPooling2DOpDescriptor
-  init(kernelWidth:kernelHeight:strideInX:strideInY:dilationRateInX:dilationRateInY:paddingLeft:paddingRight:paddingTop:paddingBottom:paddingStyle:dataLayout:) 

Initializer

# init(kernelWidth:kernelHeight:strideInX:strideInY:dilationRateInX:dilationRateInY:paddingLeft:paddingRight:paddingTop:paddingBottom:paddingStyle:dataLayout:)

Creates a 2D pooling descriptor with given values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
convenience init?(
    kernelWidth: Int,
    kernelHeight: Int,
    strideInX: Int,
    strideInY: Int,
    dilationRateInX: Int,
    dilationRateInY: Int,
    paddingLeft: Int,
    paddingRight: Int,
    paddingTop: Int,
    paddingBottom: Int,
    paddingStyle: MPSGraphPaddingStyle,
    dataLayout: MPSGraphTensorNamedDataLayout
)
```

## Parameters 

`kernelWidth`  

See `kernelWidth` property.

`kernelHeight`  

See `kernelHeight` property.

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

## Return Value

The descriptor on autoreleasepool.

