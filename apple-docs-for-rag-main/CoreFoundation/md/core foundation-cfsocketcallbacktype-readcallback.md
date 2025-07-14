

- Core Foundation
- CFSocketCallBackType
-  readCallBack 

Type Property

# readCallBack

The callback is called when data is available to be read or a new connection is waiting to be accepted. The data is not automatically read; the callback must read the data itself.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var readCallBack: CFSocketCallBackType { get }
```

## See Also

### Constants

static var acceptCallBack: CFSocketCallBackType

New connections will be automatically accepted and the callback is called with the data argument being a pointer to a CFSocketNativeHandle of the child socket. This callback is usable only with listening sockets.

static var dataCallBack: CFSocketCallBackType

Incoming data will be read in chunks in the background and the callback is called with the data argument being a CFData object containing the read data.

static var connectCallBack: CFSocketCallBackType

static var writeCallBack: CFSocketCallBackType

The callback is called when the socket is writable. This callback type may be useful when large amounts of data are being sent rapidly over the socket and you want a notification when there is space in the kernel buffers for more data.

