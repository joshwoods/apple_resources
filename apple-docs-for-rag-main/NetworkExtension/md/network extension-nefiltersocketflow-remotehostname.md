

- Network Extension
- NEFilterSocketFlow
-  remoteHostname 

Instance Property

# remoteHostname

The flow’s remote hostname, if applicable.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var remoteHostname: String? { get }
```

## Discussion

This property is only populated for flows originating from create-by-name APIs like URLSession or Network.

## See Also

### Getting socket flow properties

var remoteEndpoint: NWEndpoint?

An object containing details about the socket’s remote endpoint.

Deprecated

class NEFilterFlow

The abstract base class for types that represent flows of network data.

var localEndpoint: NWEndpoint?

An object containing details about the socket’s local endpoint.

Deprecated

var socketFamily: Int32

The protocol family of the socket.

var socketType: Int32

The type of the socket.

var socketProtocol: Int32

The protocol of the socket.

