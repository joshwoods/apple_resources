

- Foundation
- NSXPCConnection
-  exportedObject 

Instance Property

# exportedObject

An exported object for the connection.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var exportedObject: Any? { get set }
```

## Discussion

Messages sent to the remoteObjectProxy() object from the other side of the connection are dispatched to this object. Messages delivered to exported objects are serialized and sent on a non-main queue. The receiver is responsible for handling the messages on a different queue or thread if it is required.

## See Also

### Managing the connection interface

var serviceName: String?

The name of the XPC service that this connection was configured to connect to.

var endpoint: NSXPCListenerEndpoint

If the connection was created with an NSXPCListenerEndpoint object, returns the endpoint object used.

var exportedInterface: NSXPCInterface?

The NSXPCInterface object that describes the protocol for the exported object on this connection.

var remoteObjectInterface: NSXPCInterface?

Defines the NSXPCInterface object that describes the protocol for the object represented by the `remoteObjectProxy`.

var remoteObjectProxy: Any

Returns a proxy for the remote object (that is, the `exportedObject` from the other side of this connection).

