

- System
- Errno
-  noSuchAddressOrDevice 

Type Property

# noSuchAddressOrDevice

No such device or address.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var noSuchAddressOrDevice: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

Input or output on a special file referred to a device that didn’t exist, or made a request beyond the limits of the device. This error may also occur when, for example, a tape drive isn’t online or when there isn’t a disk pack loaded on a drive.

The corresponding C error is `ENXIO`.

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

static var notBlockDevice: Errno

Not a block device.

static var operationNotSupportedByDevice: Errno

Operation not supported by device.

