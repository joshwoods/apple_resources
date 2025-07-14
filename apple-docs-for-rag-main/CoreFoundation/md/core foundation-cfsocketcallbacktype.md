

- Core Foundation
-  CFSocketCallBackType 

Structure

# CFSocketCallBackType

Types of socket activity that can cause the callback function of a CFSocket object to be called.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFSocketCallBackType
```

## Overview

The callback types for which a callback is made is determined when the CFSocket object is created, such as with CFSocketCreate(_:_:_:_:_:_:_:), or later with CFSocketEnableCallBacks(_:_:) and CFSocketDisableCallBacks(_:_:).

The `kCFSocketReadCallBack`, `kCFSocketAcceptCallBack`, and `kCFSocketDataCallBack` callbacks are mutually exclusive.

### Version-Notes

`kCFSocketWriteCallBack` is available in macOS 10.2 and later.

## Topics

### Constants

static var readCallBack: CFSocketCallBackType

The callback is called when data is available to be read or a new connection is waiting to be accepted. The data is not automatically read; the callback must read the data itself.

static var acceptCallBack: CFSocketCallBackType

New connections will be automatically accepted and the callback is called with the data argument being a pointer to a CFSocketNativeHandle of the child socket. This callback is usable only with listening sockets.

static var dataCallBack: CFSocketCallBackType

Incoming data will be read in chunks in the background and the callback is called with the data argument being a CFData object containing the read data.

static var connectCallBack: CFSocketCallBackType

static var writeCallBack: CFSocketCallBackType

The callback is called when the socket is writable. This callback type may be useful when large amounts of data are being sent rapidly over the socket and you want a notification when there is space in the kernel buffers for more data.

### Initializers

init(rawValue: CFOptionFlags)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

CFSocket Flags

Flags that can be set on a CFSocket object to control its behavior.

enum CFSocketError

Error codes for many CFSocket functions.

