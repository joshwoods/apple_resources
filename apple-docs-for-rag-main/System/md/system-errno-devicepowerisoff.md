

- System
- Errno
-  devicePowerIsOff 

Type Property

# devicePowerIsOff

Device power is off.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var devicePowerIsOff: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The corresponding C error is `EPWROFF`.

## See Also

### Device Errors

static var deviceError: Errno

Device error.

static var inappropriateIOCTLForDevice: Errno

Inappropriate control function.

static var ioError: Errno

Input/output error.

static var noSuchAddressOrDevice: Errno

No such device or address.

static var notBlockDevice: Errno

Not a block device.

static var operationNotSupportedByDevice: Errno

Operation not supported by device.

