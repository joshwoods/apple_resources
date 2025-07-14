

- Metal Performance Shaders Graph
- MPSGraphStencilOpDescriptor
-  offsets 

Instance Property

# offsets

An array of length four that determines from which offset to start reading the input tensor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var offsets: [NSNumber] { get set }
```

## Discussion

Only used when `paddingStyle` is `MPSGraphPaddingStyleExplicitOffset`. For example zero offset means that the first stencil window will align its top-left corner (in 4 dimensions) to the top-left corner of the input tensor. Default value: `@[ @0, @0, @0, @0 ]`

