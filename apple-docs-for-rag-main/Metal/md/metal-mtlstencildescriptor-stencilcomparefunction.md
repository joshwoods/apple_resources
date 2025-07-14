

- Metal
- MTLStencilDescriptor
-  stencilCompareFunction 

Instance Property

# stencilCompareFunction

The comparison that is performed between the masked reference value and a masked value in the stencil attachment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var stencilCompareFunction: MTLCompareFunction { get set }
```

## Discussion

For example, if `stencilCompareFunction` is MTLCompareFunction.less, then the stencil test passes if the masked reference value is less than the masked stored stencil value. The default value is MTLCompareFunction.always, which indicates that the stencil test always passes.

The stored stencil value and the reference value are both *masked* by performing a logical AND operation with the readMask value before the comparison takes place. For more information on possible values, see MTLCompareFunction.

## See Also

### Related Documentation

func setStencilReferenceValue(UInt32)

Configures the same comparison value for front- and back-facing primitives.

**Required**

### Specifying Stencil Functions and Operations

var stencilFailureOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when the stencil test fails.

var depthFailureOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when the stencil test passes, but the depth test fails.

var depthStencilPassOperation: MTLStencilOperation

The operation that is performed to update the values in the stencil attachment when both the stencil test and the depth test pass.

