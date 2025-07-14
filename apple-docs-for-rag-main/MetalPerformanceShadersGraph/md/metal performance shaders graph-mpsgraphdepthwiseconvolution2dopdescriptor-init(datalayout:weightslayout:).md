

- Metal Performance Shaders Graph
- MPSGraphDepthwiseConvolution2DOpDescriptor
-  init(dataLayout:weightsLayout:) 

Initializer

# init(dataLayout:weightsLayout:)

Creates a 2D-depthwise convolution descriptor with given properties and default values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
convenience init?(
    dataLayout: MPSGraphTensorNamedDataLayout,
    weightsLayout: MPSGraphTensorNamedDataLayout
)
```

## Parameters 

`dataLayout`  

See `dataLayout` property.

`weightsLayout`  

See `weightsLayout` property.

## Return Value

The descriptor on autoreleasepool.

