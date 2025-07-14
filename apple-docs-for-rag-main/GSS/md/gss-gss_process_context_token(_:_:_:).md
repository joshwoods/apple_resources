

- GSS
-  gss_process_context_token(\_:\_:\_:) 

Function

# gss_process_context_token(\_:\_:\_:)

Processes a token from a peer asynchronously.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_process_context_token(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: gss_ctx_id_t,
    _ token_buffer: gss_buffer_t
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context that should handle the token.

`token_buffer`  

The token to process.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Discussion

Normally, contexts exchange tokens during the initialization process, using gss_init_sec_context(_:_:_:_:_:_:_:_:_:_:_:_:_:) and in the initiator and gss_accept_sec_context(_:_:_:_:_:_:_:_:_:_:_:) in the acceptor. Occasionally, a mechanism needs to send a token asynchronously, for example after a call to the gss_delete_sec_context(_:_:_:) function when you supply an output token buffer. The `gss_process_context_token` function provides a means to supply a token received from a peer to the context unexpectedly.

## See Also

### Creation and Deletion

func gss_init_sec_context(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_name_t, gss_OID?, OM_uint32, OM_uint32, gss_channel_bindings_t?, gss_buffer_t?, UnsafeMutablePointer&lt;gss_OID?>?, gss_buffer_t, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Initiates a security context with a peer.

func gss_accept_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_cred_id_t?, gss_buffer_t?, gss_channel_bindings_t?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;gss_OID?>?, gss_buffer_t, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_id_t?>?) -> OM_uint32

Accepts a security context initiated by a peer.

func gss_delete_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_buffer_t?) -> OM_uint32

Deletes a security context.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

func gss_set_sec_context_option(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t>?, gss_OID, gss_buffer_t?) -> OM_uint32

Sets an option on a context.

