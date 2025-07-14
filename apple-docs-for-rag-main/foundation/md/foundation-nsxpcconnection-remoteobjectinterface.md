

- Foundation
- NSXPCConnection
-  remoteObjectInterface 

Instance Property

# remoteObjectInterface

Defines the NSXPCInterface object that describes the protocol for the object represented by the `remoteObjectProxy`.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var remoteObjectInterface: NSXPCInterface? { get set }
```

## Discussion

The proxy represents the `exportedObject` on the `NSXPCConnection` in the other process.

This value is required if messages are sent over this connection.

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

var remoteObjectProxy: Any

Returns a proxy for the remote object (that is, the `exportedObject` from the other side of this connection).

