

- Metal Performance Shaders Graph
- MPSGraphImToColOpDescriptor
-  init(kernelWidth:kernelHeight:strideInX:strideInY:dilationRateInX:dilationRateInY:dataLayout:) 

Initializer

# init(kernelWidth:kernelHeight:strideInX:strideInY:dilationRateInX:dilationRateInY:dataLayout:)

Creates column to image descriptor with given values for parameters.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
convenience init?(
    kernelWidth: Int,
    kernelHeight: Int,
    strideInX: Int,
    strideInY: Int,
    dilationRateInX: Int,
    dilationRateInY: Int,
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

`dataLayout`  

See `dataLayout` property.

## Return Value

A valid MPSGraphImToColOpDescriptor on autoreleasepool.

