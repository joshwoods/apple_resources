

- XPC
-  xpc_connection_get_asid(\_:) 

Function

# xpc_connection_get_asid(\_:)

Returns the audit session identifier of the remote peer.

macOS 10.7+

``` source
func xpc_connection_get_asid(_ connection: xpc_connection_t) -> au_asid_t
```

## Parameters 

`connection`  

The connection object which is to be examined.

## Return Value

The audit session ID of the remote peer at the time the connection was made.

## See Also

### Remote peer information

func xpc_connection_get_name(xpc_connection_t) -> UnsafePointer&lt;CChar>?

Returns the name of the remote service that creates the connection.

func xpc_connection_get_euid(xpc_connection_t) -> uid_t

Returns the EUID of the remote peer.

func xpc_connection_get_egid(xpc_connection_t) -> gid_t

Returns the EGID of the remote peer.

func xpc_connection_get_pid(xpc_connection_t) -> pid_t

Returns the PID of the remote peer.

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

