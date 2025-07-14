

- Core Foundation
-  CFSocketError 

Enumeration

# CFSocketError

Error codes for many CFSocket functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFSocketError
```

## Topics

### Constants

case success

The socket operation succeeded.

case error

The socket operation failed.

case timeout

The socket operation timed out.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct CFSocketCallBackType

Types of socket activity that can cause the callback function of a CFSocket object to be called.

CFSocket Flags

Flags that can be set on a CFSocket object to control its behavior.

