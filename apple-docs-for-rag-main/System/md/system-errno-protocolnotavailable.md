

- System
- Errno
-  protocolNotAvailable 

Type Property

# protocolNotAvailable

Protocol not available.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var protocolNotAvailable: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A bad option or level was specified in a `getsockopt(2)` or `setsockopt(2)` call.

The corresponding C error is `ENOPROTOOPT`.

## See Also

### Network Protocol Errors

static var protocolError: Errno

Protocol error.

static var protocolFamilyNotSupported: Errno

Protocol family not supported.

static var protocolNotSupported: Errno

Protocol not supported.

static var protocolWrongTypeForSocket: Errno

Protocol wrong for socket type.

