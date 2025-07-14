

- Metal Performance Shaders Graph
- MPSGraphPooling2DOpDescriptor
-  init(kernelWidth:kernelHeight:strideInX:strideInY:paddingStyle:dataLayout:) 

Initializer

# init(kernelWidth:kernelHeight:strideInX:strideInY:paddingStyle:dataLayout:)

Creates a 2D pooling descriptor with given values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
convenience init?(
    kernelWidth: Int,
    kernelHeight: Int,
    strideInX: Int,
    strideInY: Int,
    paddingStyle: MPSGraphPaddingStyle,
    dataLayout: MPSGraphTensorNamedDataLayout
)
```

## Parameters 

`kernelWidth`  

See `kernelWidth` property.

`kernelHeight`  

See \`kernelHeight\`\` property.

`strideInX`  

See `strideInX` property.

`strideInY`  

See `strideInY` property.

`paddingStyle`  

See `paddingStyle` property.

`dataLayout`  

See `dataLayout` property.

## Return Value

The descriptor on autoreleasepool.

