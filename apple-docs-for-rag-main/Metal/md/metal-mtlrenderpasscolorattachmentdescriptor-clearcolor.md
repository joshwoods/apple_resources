

- Metal
- MTLRenderPassColorAttachmentDescriptor
-  clearColor 

Instance Property

# clearColor

The color to use when clearing the color attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var clearColor: MTLClearColor { get set }
```

## Discussion

If the loadAction property of the attachment is set to MTLLoadAction.clear, then at the start of a render pass, the GPU fills the texture with the value stored in the clearColor property. Otherwise, the GPU ignores the clearColor property.

The clearColor property represents a set of RGBA components. The default value is `(0.0, 0.0, 0.0, 1.0)` (black). Use the MTLClearColorMake(_:_:_:_:) function to construct a MTLClearColor value.

## See Also

### Specifying Clearing Value

func MTLClearColorMake(Double, Double, Double, Double) -> MTLClearColor

Returns a color value used to clear a color attachment.

