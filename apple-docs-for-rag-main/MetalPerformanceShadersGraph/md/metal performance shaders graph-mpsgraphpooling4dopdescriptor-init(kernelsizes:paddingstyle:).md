

- Metal Performance Shaders Graph
- MPSGraphPooling4DOpDescriptor
-  init(kernelSizes:paddingStyle:) 

Initializer

# init(kernelSizes:paddingStyle:)

Creates a 4D pooling descriptor with default values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
convenience init?(
    kernelSizes: [NSNumber],
    paddingStyle: MPSGraphPaddingStyle
)
```

## Parameters 

`kernelSizes`  

See `kernelSizes` property.

`paddingStyle`  

See `paddingStyle` property.

## Return Value

The descriptor on autoreleasepool.

