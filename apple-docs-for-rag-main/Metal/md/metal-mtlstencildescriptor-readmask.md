

- Metal
- MTLStencilDescriptor
-  readMask 

Instance Property

# readMask

A bitmask that determines from which bits that stencil comparison tests can read.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var readMask: UInt32 { get set }
```

## Discussion

The readMask bits are used for logical AND operations to both the stored stencil value and the reference value.

The least significant bits of the read mask are used. The default value is all ones. A logical AND operation with the default readMask does not change the value.

## See Also

### Related Documentation

func setStencilReferenceValue(UInt32)

Configures the same comparison value for front- and back-facing primitives.

**Required**

### Specifying Stencil Bit Mask Properties

var writeMask: UInt32

A bitmask that determines to which bits that stencil operations can write.

