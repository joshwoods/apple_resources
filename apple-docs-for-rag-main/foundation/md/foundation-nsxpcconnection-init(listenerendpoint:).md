

- Foundation
- NSXPCConnection
-  init(listenerEndpoint:) 

Initializer

# init(listenerEndpoint:)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in another process, identified by an NSXPCListenerEndpoint object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(listenerEndpoint endpoint: NSXPCListenerEndpoint)
```

## Parameters 

`endpoint`  

The desired listener endpoint for the service.

## See Also

### Related Documentation

Daemons and Services Programming Guide

### Creating a connection

init(machServiceName: String, options: NSXPCConnection.Options)

Initializes an NSXPCConnection object to connect to a LaunchAgent or LaunchDaemon with a name advertised in a `launchd.plist`.

struct Options

Options that you can pass to a connection.

init(serviceName: String)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in an XPC service, identified by a service name.

