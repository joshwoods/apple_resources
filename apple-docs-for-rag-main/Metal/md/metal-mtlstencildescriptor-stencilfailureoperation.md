

- Metal
- MTLStencilDescriptor
-  stencilFailureOperation 

Instance Property

# stencilFailureOperation

The operation that is performed to update the values in the stencil attachment when the stencil test fails.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var stencilFailureOperation: MTLStencilOperation { get set }
```

## Discussion

The default value is MTLStencilOperation.keep, which does not change the current stencil value. For more information on possible values, see MTLStencilOperation.

When the stencil test fails for a pixel, its incoming color, depth, or stencil values are discarded.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Specifying Stencil Functions and Operations

var depthFailureOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when the stencil test passes, but the depth test fails.

var depthStencilPassOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when both the stencil test and the depth test pass.

var stencilCompareFunction: MTLCompareFunction

The comparison that is performed between the masked reference value and a masked value in the stencil attachment.

