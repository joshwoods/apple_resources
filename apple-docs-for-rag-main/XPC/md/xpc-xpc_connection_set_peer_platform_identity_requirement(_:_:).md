

- XPC
-  xpc_connection_set_peer_platform_identity_requirement(\_:\_:) 

Function

# xpc_connection_set_peer_platform_identity_requirement(\_:\_:)

Sets a requirement that the executable for the peer process has a valid code signature that identifies it as an Apple-signed binary with the given signing identifier.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+

``` source
func xpc_connection_set_peer_platform_identity_requirement(
    _ connection: xpc_connection_t,
    _ signing_identifier: UnsafePointer?
) -> Int32
```

## Parameters 

`connection`  

The XPC connection.

`signing_identifier`  

The code-signing identifier for the peer process’s executable. This value is typically a Bundle ID for apps and extensions. Pass `NULL` to indicate that any Apple-signed binary is acceptable.

## Return Value

On success, `0`. Otherwise, a value from Errors.

## Discussion

When you set this requirement on a connection, the operating system checks that peer process satisfies the requirement every time it sends a message to your process. If the peer process initiated the connection and its executable doesn’t satisfy the lightweight code requirement, then you don’t receive a message and the operating system doesn’t call your event handler. If your process sent a message to its peer expecting a reply, and its executable doesn’t have the requested entitlement, then you don’t receive a reply and the operating system delivers XPC_ERROR_PEER_CODE_SIGNING_REQUIREMENT instead.

Important

It’s an error to call this function multiple times for the same connection, or to call multiple functions that set code-signing requirements on the same connection. If you do, then the operating system terminates your process.

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

func xpc_connection_get_asid(xpc_connection_t) -> au_asid_t

Returns the audit session identifier of the remote peer.

func xpc_connection_set_peer_entitlement_exists_requirement(xpc_connection_t, UnsafePointer&lt;CChar>) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature that contains an entitlement.

func xpc_connection_set_peer_entitlement_matches_value_requirement(xpc_connection_t, UnsafePointer&lt;CChar>, xpc_object_t) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature that contains an entitlement with a specific value.

func xpc_connection_set_peer_lightweight_code_requirement(xpc_connection_t, xpc_object_t) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature that matches the lightweight code requirement.

func xpc_connection_set_peer_team_identity_requirement(xpc_connection_t, UnsafePointer&lt;CChar>?) -> Int32

Sets a requirement that the executable for the peer process has a valid code signature and is signed by the same team identifier as the calling process.

func xpc_connection_set_peer_code_signing_requirement(xpc_connection_t, UnsafePointer&lt;CChar>) -> Int32

