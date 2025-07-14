

- Metal Performance Shaders Graph
- MPSGraphImToColOpDescriptor
-  init(kernelWidth:kernelHeight:strideInX:strideInY:dilationRateInX:dilationRateInY:paddingLeft:paddingRight:paddingTop:paddingBottom:dataLayout:) 

Initializer

# init(kernelWidth:kernelHeight:strideInX:strideInY:dilationRateInX:dilationRateInY:paddingLeft:paddingRight:paddingTop:paddingBottom:dataLayout:)

Creates an image to column descriptor with given values for parameters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

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

`dataLayout`  

See `dataLayout` property.

## Return Value

A valid MPSGraphImToColOpDescriptor on autoreleasepool.

