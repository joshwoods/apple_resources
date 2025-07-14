

- XPC
-  xpc_connection_t 

Type Alias

# xpc_connection_t

A type that represents a connection to a named service.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_connection_t = xpc_object_t
```

## See Also

### Creation

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

var XPC_CONNECTION_MACH_SERVICE_PRIVILEGED: Int32

A flag that indicates the job advertising the service name belongs to a launch daemon rather than a launch agent.

