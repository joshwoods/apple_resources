

- Foundation
- NSXPCConnection
-  remoteObjectProxyWithErrorHandler(\_:) 

Instance Method

# remoteObjectProxyWithErrorHandler(\_:)

Returns a proxy for the remote object (that is, the object exported from the other side of this connection) with the specified error handler.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remoteObjectProxyWithErrorHandler(_ handler: @escaping (any Error) -> Void) -> Any
```

## Discussion

See descriptions in NSXPCProxyCreating for more details.

## See Also

### Working with proxy objects

func synchronousRemoteObjectProxyWithErrorHandler((any Error) -> Void) -> Any

