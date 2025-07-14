

- GSS
-  gss_set_sec_context_option(\_:\_:\_:\_:) 

Function

# gss_set_sec_context_option(\_:\_:\_:\_:)

Sets an option on a context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_set_sec_context_option(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: UnsafeMutablePointer?,
    _ object: gss_OID,
    _ value: gss_buffer_t?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context to alter.

`object`  

An object identifier that indicates what part of the context to alter.

`value`  

A new value for the indicated object.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

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

func gss_process_context_token(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t) -> OM_uint32

Processes a token from a peer asynchronously.

