

- GSS
-  gss_delete_sec_context(\_:\_:\_:) 

Function

# gss_delete_sec_context(\_:\_:\_:)

Deletes a security context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_delete_sec_context(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: UnsafeMutablePointer,
    _ output_token: gss_buffer_t?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context to be deleted.

`output_token`  

A buffer that the function may fill with a token to send to the peer application. Typically, you pass GSS_C_NO_BUFFER, indicating that no token is desired, and simply call upon the deletion function to operate locally on both sides of the connection. If a token is created, pass it to the remote peer, and free its memory with a call to gss_release_buffer(_:_:).

## Return Value

A status code set to GSS_S_COMPLETE on completion, or GSS_S_NO_CONTEXT if no context was supplied.

## Discussion

This function purges the context and all of its resources from memory, and frees all of its memory.

## See Also

### Creation and Deletion

func gss_init_sec_context(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_name_t, gss_OID?, OM_uint32, OM_uint32, gss_channel_bindings_t?, gss_buffer_t?, UnsafeMutablePointer&lt;gss_OID?>?, gss_buffer_t, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Initiates a security context with a peer.

func gss_accept_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_cred_id_t?, gss_buffer_t?, gss_channel_bindings_t?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;gss_OID?>?, gss_buffer_t, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_id_t?>?) -> OM_uint32

Accepts a security context initiated by a peer.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

func gss_process_context_token(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t) -> OM_uint32

Processes a token from a peer asynchronously.

func gss_set_sec_context_option(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t>?, gss_OID, gss_buffer_t?) -> OM_uint32

Sets an option on a context.

