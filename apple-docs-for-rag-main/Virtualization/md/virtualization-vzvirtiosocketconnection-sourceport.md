

- Virtualization
- VZVirtioSocketConnection
-  sourcePort 

Instance Property

# sourcePort

The port number of the system that opened the connection.

macOS 11.0+

``` source
var sourcePort: UInt32 { get }
```

## Discussion

When the guest operating system opens a connection, this property contains the port number that the guest specified. When you open a connection to the guest operating system from your VZVirtioSocketDevice object, this property contains a randomly generated port number.

## See Also

### Getting the connection details

var destinationPort: UInt32

The destination port number of the connection.

var fileDescriptor: Int32

The file descriptor to use when sending data.

