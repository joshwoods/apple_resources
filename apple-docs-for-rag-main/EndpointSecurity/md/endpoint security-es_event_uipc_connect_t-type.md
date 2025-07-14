

- Endpoint Security
- es_event_uipc_connect_t
-  type 

Instance Property

# type

The type of the socket.

Mac CatalystmacOS

``` source
var type: Int32
```

## Discussion

See the man page for `socket(2)` for a list of available type values.

## See Also

### Inspecting Event Properties

var file: UnsafeMutablePointer&lt;es_file_t>

The socket file bound to the socket.

var domain: Int32

The communications domain of the socket.

var `protocol`: Int32

The protocol of the socket.

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An unused field reserved for future use.

