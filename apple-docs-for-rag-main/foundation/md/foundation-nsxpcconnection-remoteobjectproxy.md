

- Foundation
- NSXPCConnection
-  remoteObjectProxy 

Instance Property

# remoteObjectProxy

Returns a proxy for the remote object (that is, the `exportedObject` from the other side of this connection).

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var remoteObjectProxy: Any { get }
```

## Discussion

See descriptions in NSXPCProxyCreating for more details.

## See Also

### Managing the connection interface

var serviceName: String?

The name of the XPC service that this connection was configured to connect to.

var endpoint: NSXPCListenerEndpoint

If the connection was created with an NSXPCListenerEndpoint object, returns the endpoint object used.

var exportedInterface: NSXPCInterface?

The NSXPCInterface object that describes the protocol for the exported object on this connection.

var exportedObject: Any?

An exported object for the connection.

var remoteObjectInterface: NSXPCInterface?

Defines the NSXPCInterface object that describes the protocol for the object represented by the `remoteObjectProxy`.

