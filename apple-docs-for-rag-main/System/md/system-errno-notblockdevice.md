

- System
- Errno
-  notBlockDevice 

Type Property

# notBlockDevice

Not a block device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var notBlockDevice: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted a block device operation on a nonblock device or file.

The corresponding C error is `ENOTBLK`.

## See Also

### Device Errors

static var deviceError: Errno

Device error.

static var devicePowerIsOff: Errno

Device power is off.

static var inappropriateIOCTLForDevice: Errno

Inappropriate control function.

static var ioError: Errno

Input/output error.

static var noSuchAddressOrDevice: Errno

No such device or address.

static var operationNotSupportedByDevice: Errno

Operation not supported by device.

