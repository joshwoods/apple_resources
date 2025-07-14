

- System
- Errno
-  operationNotSupportedByDevice 

Type Property

# operationNotSupportedByDevice

Operation not supported by device.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var operationNotSupportedByDevice: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

You attempted to apply an inappropriate function to a device; for example, trying to read a write-only device such as a printer.

The corresponding C error is `ENODEV`.

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

static var notBlockDevice: Errno

Not a block device.

