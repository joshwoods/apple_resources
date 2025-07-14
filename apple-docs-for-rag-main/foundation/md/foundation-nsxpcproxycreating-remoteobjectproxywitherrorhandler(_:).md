

- Foundation
- NSXPCProxyCreating
-  remoteObjectProxyWithErrorHandler(\_:) 

Instance Method

# remoteObjectProxyWithErrorHandler(\_:)

Returns a proxy object that invokes the error handling block if an error occurs on the connection.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remoteObjectProxyWithErrorHandler(_ handler: @escaping (any Error) -> Void) -> Any
```

**Required**

## Parameters 

`handler`  

The error handling block that the proxy object should call when an error occurs while waiting for a reply.

## Discussion

If the message sent to the proxy has a reply handler, then either the error handler or the reply handler is called exactly once.

The resulting proxy object conforms to the `NSXPCProxyCreating` protocol.

