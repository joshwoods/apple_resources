

- Network Extension
- NEFilterSocketFlow
-  localEndpoint Deprecated

Instance Property

# localEndpoint

An object containing details about the socket’s local endpoint.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var localEndpoint: NWEndpoint? { get }
```

## Discussion

This endpoint object may be `nil` when the system calls your handleNewFlow(_:) method; if so, receiving network data populates the object. In such a case, the filter may still perform filtering, based on its socket type, socket family, or socket protocol.

## See Also

### Getting socket flow properties

var remoteEndpoint: NWEndpoint?

An object containing details about the socket’s remote endpoint.

Deprecated

var remoteHostname: String?

The flow’s remote hostname, if applicable.

class NEFilterFlow

The abstract base class for types that represent flows of network data.

var socketFamily: Int32

The protocol family of the socket.

var socketType: Int32

The type of the socket.

var socketProtocol: Int32

The protocol of the socket.

