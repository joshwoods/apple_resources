

- Metal Performance Shaders Graph
- MPSGraphPooling4DOpDescriptor
-  init(kernelSizes:strides:dilationRates:paddingValues:paddingStyle:) 

Initializer

# init(kernelSizes:strides:dilationRates:paddingValues:paddingStyle:)

Creates a 4D pooling descriptor with given values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
convenience init?(
    kernelSizes: [NSNumber],
    strides: [NSNumber],
    dilationRates: [NSNumber],
    paddingValues: [NSNumber],
    paddingStyle: MPSGraphPaddingStyle
)
```

## Parameters 

`kernelSizes`  

See `kernelSizes` property.

`strides`  

See `strides` property.

`dilationRates`  

See `dilationRates` property.

`paddingValues`  

See `paddingValues` property.

`paddingStyle`  

See `paddingStyle` property.

## Return Value

The descriptor on autoreleasepool.

