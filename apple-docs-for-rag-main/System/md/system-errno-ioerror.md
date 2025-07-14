

- System
- Errno
-  ioError 

Type Property

# ioError

Input/output error.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var ioError: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

Some physical input or output error occurred. This error isn’t reported until you attempt a subsequent operation on the same file descriptor, and the error may be lost (overwritten) by subsequent errors.

The corresponding C error is `EIO`.

## See Also

### Device Errors

static var deviceError: Errno

Device error.

static var devicePowerIsOff: Errno

Device power is off.

static var inappropriateIOCTLForDevice: Errno

Inappropriate control function.

static var noSuchAddressOrDevice: Errno

No such device or address.

static var notBlockDevice: Errno

Not a block device.

static var operationNotSupportedByDevice: Errno

Operation not supported by device.

