

- System
- Errno
-  inappropriateIOCTLForDevice 

Type Property

# inappropriateIOCTLForDevice

Inappropriate control function.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var inappropriateIOCTLForDevice: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted a control function that can’t be performed on the specified file or device. For information about control functions, see `ioctl(2)`.

The corresponding C error is `ENOTTY`.

## See Also

### Device Errors

static var deviceError: Errno

Device error.

static var devicePowerIsOff: Errno

Device power is off.

static var ioError: Errno

Input/output error.

static var noSuchAddressOrDevice: Errno

No such device or address.

static var notBlockDevice: Errno

Not a block device.

static var operationNotSupportedByDevice: Errno

Operation not supported by device.

