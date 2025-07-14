

- Metal Performance Shaders Graph
- MPSGraphStencilOpDescriptor
-  init(reductionMode:offsets:strides:dilationRates:explicitPadding:boundaryMode:paddingStyle:paddingConstant:) 

Initializer

# init(reductionMode:offsets:strides:dilationRates:explicitPadding:boundaryMode:paddingStyle:paddingConstant:)

Creates a stencil operation descriptor with given values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
convenience init?(
    reductionMode: MPSGraphReductionMode,
    offsets: [NSNumber],
    strides: [NSNumber],
    dilationRates: [NSNumber],
    explicitPadding: [NSNumber],
    boundaryMode: MPSGraphPaddingMode,
    paddingStyle: MPSGraphPaddingStyle,
    paddingConstant: Float
)
```

## Parameters 

`reductionMode`  

See `reductionMode` property.

`offsets`  

See `offsets` property.

`strides`  

See `strides` property.

`dilationRates`  

See `dilationRates` property.

`explicitPadding`  

See `explicitPadding` property.

`boundaryMode`  

See `boundaryMode` property.

`paddingStyle`  

See `paddingStyle` property.

`paddingConstant`  

See `paddingConstant` property.

## Return Value

A valid MPSGraphStencilOpDescriptor object

