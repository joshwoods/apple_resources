

- System
- Errno
-  protocolWrongTypeForSocket 

Type Property

# protocolWrongTypeForSocket

Protocol wrong for socket type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var protocolWrongTypeForSocket: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A protocol was specified that doesn’t support the semantics of the socket type requested. For example, you can’t use the ARPA Internet UDP protocol with type `SOCK_STREAM`.

The corresponding C error is `EPROTOTYPE`.

## See Also

### Network Protocol Errors

static var protocolError: Errno

Protocol error.

static var protocolFamilyNotSupported: Errno

Protocol family not supported.

static var protocolNotAvailable: Errno

Protocol not available.

static var protocolNotSupported: Errno

Protocol not supported.

