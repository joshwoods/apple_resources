

- Metal
- MTLStencilDescriptor
-  writeMask 

Instance Property

# writeMask

A bitmask that determines to which bits that stencil operations can write.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var writeMask: UInt32 { get set }
```

## Discussion

writeMask are used for logical AND operations to values that are going to be written into a stencil attachment as the result of a stencil operation.

The least significant bits of the write mask are used. The default value is all ones. A logical AND operation with the default writeMask does not change the value.

## See Also

### Specifying Stencil Bit Mask Properties

var readMask: UInt32

A bitmask that determines from which bits that stencil comparison tests can read.

