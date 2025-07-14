

- Metal Performance Shaders Graph
- MPSGraphStencilOpDescriptor
-  explicitPadding 

Instance Property

# explicitPadding

The property that defines padding values for spatial dimensions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var explicitPadding: [NSNumber] { get set }
```

## Discussion

Must be eight numbers, two for each spatial dimension. For example `paddingValues[0]` defines the explicit padding amount before the first spatial dimension (slowest running index of spatial dimensions), `paddingValues[1]` defines the padding amount after the first spatial dimension etc. Used only when `paddingStyle = MPSGraphPaddingStyleExplicit`. Default value: `@[ @0, @0, @0, @0, @0, @0, @0, @0 ]`

