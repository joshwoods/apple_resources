

- Foundation
- NSXPCListenerDelegate
-  listener(\_:shouldAcceptNewConnection:) 

Instance Method

# listener(\_:shouldAcceptNewConnection:)

Accepts or rejects a new connection to the listener.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func listener(
    _ listener: NSXPCListener,
    shouldAcceptNewConnection newConnection: NSXPCConnection
) -> Bool
```

## Discussion

To accept the connection, first configure the connection if desired, then call resume() on the new connection, then return true.

To reject the connect, return a value of false. This causes the connection object to be invalidated.

In this method, you can also set up properties on the connection object, such as its exported object and interfaces. Be sure to call resume() when you are finished configuring the connection object and are ready for it to receive messages.

## See Also

### Related Documentation

Daemons and Services Programming Guide

