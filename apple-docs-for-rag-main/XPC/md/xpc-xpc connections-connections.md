

- XPC
-  XPC connections 

API Collection

# XPC connections

Create and manage connections to services using connection-based APIs.

## Overview

Use these APIs to work with XPC connections and related types — for example, when a framework function that you call returns an xpc_connection_t.

But, in most situations, the listener- and session-based APIs are a better choice for designing XPC communication protocols. For more information, see Creating XPC services.

## Topics

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

var XPC_CONNECTION_MACH_SERVICE_PRIVILEGED: Int32

A flag that indicates the job advertising the service name belongs to a launch daemon rather than a launch agent.

### Event handling

func xpc_connection_set_event_handler(xpc_connection_t, xpc_handler_t)

Sets the event handler block for the connection.

typealias xpc_handler_t

The type of block that the XPC connection APIs accept.

typealias xpc_connection_handler_t

The type of the function to invoke for a bundled XPC service when there’s a new connection on the service.

### Life cycle

func xpc_main(xpc_connection_handler_t) -> Never

Starts listening for incoming connections and processes them with the specified event handler.

func xpc_connection_activate(xpc_connection_t)

Activates a new connection.

func xpc_connection_suspend(xpc_connection_t)

Suspends the connection so the event handler block doesn’t fire and the connection doesn’t attempt to send any messages it has in its queue.

func xpc_connection_resume(xpc_connection_t)

Resumes a suspended connection.

func xpc_connection_cancel(xpc_connection_t)

Cancels the connection and ensures that its event handler doesn’t fire again.

func xpc_transaction_begin()

Informs the XPC runtime when a transaction begins, indicating that the service isn’t idle.

func xpc_transaction_end()

Informs the XPC runtime when a transaction ends.

func xpc_connection_copy_invalidation_reason(xpc_connection_t) -> UnsafeMutablePointer&lt;CChar>?

### Messages

func xpc_connection_send_message(xpc_connection_t, xpc_object_t)

Sends a message over the connection to the destination service.

func xpc_connection_send_barrier(xpc_connection_t, () -> Void)

Issues a barrier against the connection’s message-send activity.

func xpc_connection_send_message_with_reply(xpc_connection_t, xpc_object_t, dispatch_queue_t?, xpc_handler_t)

Sends a message over the connection to the destination service and associates a handler to invoke when the remote service sends a reply message.

func xpc_connection_send_message_with_reply_sync(xpc_connection_t, xpc_object_t) -> xpc_object_t

Sends a message over the connection and blocks the caller until it receives a reply.

func xpc_main(xpc_connection_handler_t) -> Never

Starts listening for incoming connections and processes them with the specified event handler.

### Remote peer information

func xpc_connection_get_name(xpc_connection_t) -> UnsafePointer&lt;CChar>?

Returns the name of the remote service that creates the connection.

func xpc_connection_get_euid(xpc_connection_t) -> uid_t

Returns the EUID of the remote peer.

func xpc_connection_get_egid(xpc_connection_t) -> gid_t

Returns the EGID of the remote peer.

func xpc_connection_get_pid(xpc_connection_t) -> pid_t

Returns the PID of the remote peer.

func xpc_connection_get_asid(xpc_connection_t) -> au_asid_t

Returns the audit session identifier of the remote peer.

func xpc_connection_set_peer_entitlement_exists_requirement(xpc_connection_t, UnsafePointer&lt;CChar>) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature that contains an entitlement.

func xpc_connection_set_peer_entitlement_matches_value_requirement(xpc_connection_t, UnsafePointer&lt;CChar>, xpc_object_t) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature that contains an entitlement with a specific value.

func xpc_connection_set_peer_lightweight_code_requirement(xpc_connection_t, xpc_object_t) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature that matches the lightweight code requirement.

func xpc_connection_set_peer_platform_identity_requirement(xpc_connection_t, UnsafePointer&lt;CChar>?) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature that identifies it as an Apple-signed binary with the given signing identifier.

func xpc_connection_set_peer_team_identity_requirement(xpc_connection_t, UnsafePointer&lt;CChar>?) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature and is signed by the same team identifier as the calling process.

func xpc_connection_set_peer_code_signing_requirement(xpc_connection_t, UnsafePointer&lt;CChar>) -> Int32

### Context

func xpc_connection_set_context(xpc_connection_t, UnsafeMutableRawPointer?)

Sets a context on the connection.

func xpc_connection_get_context(xpc_connection_t) -> UnsafeMutableRawPointer?

Returns the context for the connection.

func xpc_connection_set_finalizer_f(xpc_connection_t, xpc_finalizer_t?)

Sets the finalizer for the connection.

typealias xpc_finalizer_t

A function to invoke when tearing down a connection and freeing its context.

### Endpoints

func xpc_endpoint_create(xpc_connection_t) -> xpc_endpoint_t

Creates a new endpoint from a connection that is suitable for embedding into messages.

typealias xpc_endpoint_t

A type that represents a connection in serialized form.

### Errors

var XPC_ERROR_CONNECTION_INVALID: xpc_object_t

An error that sends to the connection’s event handler to indicate that the connection is no longer usable.

var XPC_ERROR_CONNECTION_INTERRUPTED: xpc_object_t

An error that sends to the connection’s event handler when the remote service exits.

var XPC_ERROR_TERMINATION_IMMINENT: xpc_object_t

An error that sends to a peer connection’s event handler when the XPC runtime determines that the program needs to exit and that all outstanding transactions must wind down.

## See Also

### Additional Types

XPC objects

Encapsulate data in objects that represent primitive types, collections, and more.

Utilities

Browse debugging utilities and constants to use with the XPC APIs.

