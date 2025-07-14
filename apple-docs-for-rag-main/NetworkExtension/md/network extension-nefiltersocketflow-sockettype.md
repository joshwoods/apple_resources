

- Network Extension
- NEFilterSocketFlow
-  socketType 

Instance Property

# socketType

The type of the socket.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
var socketType: Int32 { get }
```

## Discussion

Examples of socket types include `SOCK_STREAM` and `SOCK_DGRAM`.

## See Also

### Getting socket flow properties

var remoteEndpoint: NWEndpoint?

An object containing details about the socket’s remote endpoint.

Deprecated

var remoteHostname: String?

The flow’s remote hostname, if applicable.

class NEFilterFlow

The abstract base class for types that represent flows of network data.

var localEndpoint: NWEndpoint?

An object containing details about the socket’s local endpoint.

Deprecated

var socketFamily: Int32

The protocol family of the socket.

var socketProtocol: Int32

The protocol of the socket.

