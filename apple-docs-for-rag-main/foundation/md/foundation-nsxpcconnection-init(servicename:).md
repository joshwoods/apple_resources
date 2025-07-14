

- Foundation
- NSXPCConnection
-  init(serviceName:) 

Initializer

# init(serviceName:)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in an XPC service, identified by a service name.

macOS 10.8+

``` source
init(serviceName: String)
```

## Discussion

XPC services are helper processes that are usually part of your application bundle. The service should use NSXPCListener to wait for new connections.

## See Also

### Creating a connection

init(listenerEndpoint: NSXPCListenerEndpoint)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in another process, identified by an NSXPCListenerEndpoint object.

init(machServiceName: String, options: NSXPCConnection.Options)

Initializes an NSXPCConnection object to connect to a LaunchAgent or LaunchDaemon with a name advertised in a `launchd.plist`.

struct Options

Options that you can pass to a connection.

