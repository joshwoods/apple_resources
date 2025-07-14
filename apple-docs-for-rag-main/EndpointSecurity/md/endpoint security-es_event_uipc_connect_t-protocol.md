

- Endpoint Security
- es_event_uipc_connect_t
-  protocol 

Instance Property

# protocol

The protocol of the socket.

Mac CatalystmacOS

``` source
var `protocol`: Int32
```

## Discussion

See the man page for `socket(2)` for a discussion of the `protocol` parameter.

## See Also

### Inspecting Event Properties

var file: UnsafeMutablePointer&lt;es_file_t>

The socket file bound to the socket.

var domain: Int32

The communications domain of the socket.

var type: Int32

The type of the socket.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

