

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  paddingStyle 

Instance Property

# paddingStyle

The type of padding that is applied to the source tensor.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
var paddingStyle: MPSGraphPaddingStyle { get set }
```

## Discussion

If paddingStyle is `MPSGraphPaddingStyleExplicit`, `paddingLeft`, `laddingRight`, `paddingTop`, `paddingBottom`, `paddingFront` and `paddingBack` must to be specified. For all other padding styles, framework compute these values so you dont need to provide these values.

