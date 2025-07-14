

- Virtualization
- VZVirtioSocketConnection
-  fileDescriptor 

Instance Property

# fileDescriptor

The file descriptor to use when sending data.

macOS 11.0+

``` source
var fileDescriptor: Int32 { get }
```

## Discussion

To send data to the other side of the connection, write to the file descriptor. To read data from connection, read from the file descriptor. If the socket connection is closed, the value of this property is `-1`.

## See Also

### Getting the connection details

var sourcePort: UInt32

The port number of the system that opened the connection.

var destinationPort: UInt32

The destination port number of the connection.

