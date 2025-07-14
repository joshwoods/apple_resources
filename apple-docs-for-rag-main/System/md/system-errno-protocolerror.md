

- System
- Errno
-  protocolError 

Type Property

# protocolError

Protocol error.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var protocolError: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

Some protocol error occurred. This error is device-specific, but generally isn’t related to a hardware failure.

The corresponding C error is `EPROTO`.

## See Also

### Network Protocol Errors

static var protocolFamilyNotSupported: Errno

Protocol family not supported.

static var protocolNotAvailable: Errno

Protocol not available.

static var protocolNotSupported: Errno

Protocol not supported.

static var protocolWrongTypeForSocket: Errno

Protocol wrong for socket type.

