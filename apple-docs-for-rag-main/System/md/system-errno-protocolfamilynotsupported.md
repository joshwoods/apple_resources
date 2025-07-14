

- System
- Errno
-  protocolFamilyNotSupported 

Type Property

# protocolFamilyNotSupported

Protocol family not supported.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var protocolFamilyNotSupported: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

The protocol family hasn’t been configured into the system or no implementation for it exists.

The corresponding C error is `EPFNOSUPPORT`.

## See Also

### Network Protocol Errors

static var protocolError: Errno

Protocol error.

static var protocolNotAvailable: Errno

Protocol not available.

static var protocolNotSupported: Errno

Protocol not supported.

static var protocolWrongTypeForSocket: Errno

Protocol wrong for socket type.

