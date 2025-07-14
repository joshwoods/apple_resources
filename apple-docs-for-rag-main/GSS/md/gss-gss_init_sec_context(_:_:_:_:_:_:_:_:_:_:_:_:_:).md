

- GSS
-  gss_init_sec_context(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# gss_init_sec_context(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Initiates a security context with a peer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_init_sec_context(
    _ minor_status: UnsafeMutablePointer,
    _ initiator_cred_handle: gss_cred_id_t?,
    _ context_handle: UnsafeMutablePointer,
    _ target_name: gss_name_t,
    _ input_mech_type: gss_OID?,
    _ req_flags: OM_uint32,
    _ time_req: OM_uint32,
    _ input_chan_bindings: gss_channel_bindings_t?,
    _ input_token: gss_buffer_t?,
    _ actual_mech_type: UnsafeMutablePointer?,
    _ output_token: gss_buffer_t,
    _ ret_flags: UnsafeMutablePointer?,
    _ time_rec: UnsafeMutablePointer?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`initiator_cred_handle`  

The credential to use when building the context. Pass GSS_C_NO_CREDENTIAL to use the default credential for the mechanism.

`context_handle`  

A pointer the function uses to return the context. Pass GSS_C_NO_CONTEXT for first call and use the value returned by the first call in continuation calls. Release the context’s resources using the gss_delete_sec_context(_:_:_:) function when you are done with it.

`target_name`  

The name of the target acceptor, created with gss_import_name(_:_:_:_:). The name must be of a type that is supported by the mechanism, as given by gss_inquire_names_for_mech(_:_:_:).

`input_mech_type`  

The mechanism type to use. Pass GSS_C_NO_OID to try Kerberos (GSS_KRB5_MECHANISM) as a default.

`req_flags`  

Logical OR of the flags to use when building the context. See Context Services for a list of possible values.

`time_req`  

The time in seconds that the context should be valid. Use GSS_C_INDEFINITE to request the longest available time.

`input_chan_bindings`  

Channel bindings to use. Pass GSS_C_NO_CHANNEL_BINDINGS if channel bindings are not used.

`input_token`  

A token sent from the acceptor. On the first call, use GSS_C_NO_BUFFER.

`actual_mech_type`  

A pointer the function uses to return the actual mechanism used by the context. Do *not* free this object because it is held in static memory.

`output_token`  

A buffer the function fills with an opaque token that you send to the acceptor. If the length of the buffer is non-zero, a token exists and you send it to the acceptor no matter the return status, whether complete, continue, or any error condition.

`ret_flags`  

A pointer the function uses to return the actual flags supported by the context. See Context Services for a list of possible values.

`time_rec`  

A pointer the function uses to return the actual number of seconds for which the context is valid. Pass `NULL` to ignore this output.

## Return Value

A status code indicating the outcome of the call. A code of GSS_S_COMPLETE means the context is complete. A code of GSS_S_CONTINUE_NEEDED indicates the need for another round of calls. Any other return code represents an error condition. See Function Status for a complete list of possible status results.

## Discussion

Don’t call this function on a UI update thread because it may block on network activity.

## See Also

### Creation and Deletion

func gss_accept_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_cred_id_t?, gss_buffer_t?, gss_channel_bindings_t?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;gss_OID?>?, gss_buffer_t, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_id_t?>?) -> OM_uint32

Accepts a security context initiated by a peer.

func gss_delete_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_buffer_t?) -> OM_uint32

Deletes a security context.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

func gss_process_context_token(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t) -> OM_uint32

Processes a token from a peer asynchronously.

func gss_set_sec_context_option(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t>?, gss_OID, gss_buffer_t?) -> OM_uint32

Sets an option on a context.

