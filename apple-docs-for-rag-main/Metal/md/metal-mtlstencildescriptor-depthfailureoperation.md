

- Metal
- MTLStencilDescriptor
-  depthFailureOperation 

Instance Property

# depthFailureOperation

The operation that is performed to update the values in the stencil attachment when the stencil test passes, but the depth test fails.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var depthFailureOperation: MTLStencilOperation { get set }
```

## Discussion

The default value is MTLStencilOperation.keep, which does not change the current stencil value. For more information on possible values, see MTLStencilOperation.

## See Also

### Related Documentation

var depthCompareFunction: MTLCompareFunction

The comparison that is performed between a fragment’s depth value and the depth value in the attachment, which determines whether to discard the fragment.

### Specifying Stencil Functions and Operations

var stencilFailureOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when the stencil test fails.

var depthStencilPassOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when both the stencil test and the depth test pass.

var stencilCompareFunction: MTLCompareFunction

The comparison that is performed between the masked reference value and a masked value in the stencil attachment.

