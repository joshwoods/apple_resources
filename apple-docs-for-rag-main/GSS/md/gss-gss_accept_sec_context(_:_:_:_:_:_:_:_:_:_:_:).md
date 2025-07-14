

- GSS
-  gss_accept_sec_context(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# gss_accept_sec_context(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Accepts a security context initiated by a peer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_accept_sec_context(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: UnsafeMutablePointer,
    _ acceptor_cred_handle: gss_cred_id_t?,
    _ input_token: gss_buffer_t?,
    _ input_chan_bindings: gss_channel_bindings_t?,
    _ src_name: UnsafeMutablePointer?,
    _ mech_type: UnsafeMutablePointer?,
    _ output_token: gss_buffer_t,
    _ ret_flags: UnsafeMutablePointer?,
    _ time_rec: UnsafeMutablePointer?,
    _ delegated_cred_handle: UnsafeMutablePointer?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

A pointer the function uses to return the context. Pass GSS_C_NO_CONTEXT for first call and use the value returned by the first call in continuation calls. Release the context’s resources using the gss_delete_sec_context(_:_:_:) function when you are done with it.

`acceptor_cred_handle`  

The credential claimed by the acceptor. Specify GSS_C_NO_CREDENTIAL to use the default credential.

`input_token`  

The token obtained from the peer.

`input_chan_bindings`  

Channel bindings to use. Pass GSS_C_NO_CHANNEL_BINDINGS if channel bindings are not used.

`src_name`  

A pointer the function uses to return the authenticated name of the context initiator. Specify `NULL` to ignore this output.

`mech_type`  

A pointer the function uses to return the mechanism used by the context. Do *not* free this object because it is held in static memory. Specify `NULL` to ignore this output.

`output_token`  

A buffer the function fills with a token to transmit to the peer. If the buffer length is zero, there is no token to pass. Otherwise, free the token buffer’s memory using gss_release_buffer(_:_:) when you are done with it.

`ret_flags`  

A pointer the function uses to return the flags supported by the context. See Context Services for a list of possible values. Specify `NULL` to ignore this output.

`time_rec`  

A pointer the function uses to return the number of seconds for which the context is valid. Specify `NULL` to ignore this output.

`delegated_cred_handle`  

A pointer the function uses to return the credentials of the initiator. The function returns GSS_C_NO_CREDENTIAL unless the `ret_flags` parameter includes GSS_C_DELEG_FLAG. If the credential exists, release its memory with gss_release_cred(_:_:) when you are done with it.

## See Also

### Creation and Deletion

func gss_init_sec_context(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_name_t, gss_OID?, OM_uint32, OM_uint32, gss_channel_bindings_t?, gss_buffer_t?, UnsafeMutablePointer&lt;gss_OID?>?, gss_buffer_t, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Initiates a security context with a peer.

func gss_delete_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_buffer_t?) -> OM_uint32

Deletes a security context.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

func gss_process_context_token(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t) -> OM_uint32

Processes a token from a peer asynchronously.

func gss_set_sec_context_option(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t>?, gss_OID, gss_buffer_t?) -> OM_uint32

Sets an option on a context.

