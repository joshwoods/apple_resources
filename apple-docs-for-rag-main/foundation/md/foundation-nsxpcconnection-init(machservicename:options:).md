

- Foundation
- NSXPCConnection
-  init(machServiceName:options:) 

Initializer

# init(machServiceName:options:)

Initializes an NSXPCConnection object to connect to a LaunchAgent or LaunchDaemon with a name advertised in a `launchd.plist`.

macOS 10.8+

``` source
init(
    machServiceName name: String,
    options: NSXPCConnection.Options = []
)
```

## Discussion

For example, if an agent is managed with `launchd` and has a `launchd.plist` in `~/Library/LaunchAgents`, this method would create a connection to that agent. The agent should use NSXPCListener to wait for new connections.

If the connection is being made to a process that is running in a privileged Mach bootstrap context (for example, a daemon started by a `launchd` property list in `/Library/LaunchDaemons`), then pass the NSXPCConnection option.

## See Also

### Creating a connection

init(listenerEndpoint: NSXPCListenerEndpoint)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in another process, identified by an NSXPCListenerEndpoint object.

struct Options

Options that you can pass to a connection.

init(serviceName: String)

Initializes an NSXPCConnection object to connect to an NSXPCListener object in an XPC service, identified by a service name.

