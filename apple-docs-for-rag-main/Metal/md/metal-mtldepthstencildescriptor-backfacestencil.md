

- Metal
- MTLDepthStencilDescriptor
-  backFaceStencil 

Instance Property

# backFaceStencil

The stencil descriptor for back-facing primitives.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
@NSCopying
var backFaceStencil: MTLStencilDescriptor! { get set }
```

## Discussion

The default value is `nil`, which indicates the stencil test is disabled for the back-facing primitives. For more information, see MTLStencilDescriptor.

## See Also

### Specifying Stencil Descriptors for Primitives

var frontFaceStencil: MTLStencilDescriptor!

The stencil descriptor for front-facing primitives.

