

- XPC
-  XPC_CONNECTION_MACH_SERVICE_PRIVILEGED 

Global Variable

# XPC_CONNECTION_MACH_SERVICE_PRIVILEGED

A flag that indicates the job advertising the service name belongs to a launch daemon rather than a launch agent.

iOSiPadOSMac CatalystmacOS

``` source
var XPC_CONNECTION_MACH_SERVICE_PRIVILEGED: Int32 { get }
```

## Discussion

Pass this to xpc_connection_create_mach_service(_:_:_:). This flag indicates that the job advertising the service name in its `launchd.plist` needs to be in the privileged Mach bootstrap. Do this by placing your `launchd.plist` in `/Library/LaunchDaemons`.

If you specify this alongside the XPC_CONNECTION_MACH_SERVICE_LISTENER flag, this flag is a no-op.

## See Also

### Creation

typealias xpc_connection_t

A type that represents a connection to a named service.

func xpc_connection_create(UnsafePointer&lt;CChar>?, dispatch_queue_t?) -> xpc_connection_t

Creates a new connection object.

func xpc_connection_create_from_endpoint(xpc_endpoint_t) -> xpc_connection_t

Creates a new connection from the specified endpoint.

func xpc_connection_create_mach_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, UInt64) -> xpc_connection_t

Creates a new connection object that represents a Mach service.

func xpc_connection_set_target_queue(xpc_connection_t, dispatch_queue_t?)

Sets the target queue of the connection.

var XPC_CONNECTION_MACH_SERVICE_LISTENER: Int32

A flag that indicates the caller is the listener for the named service.

