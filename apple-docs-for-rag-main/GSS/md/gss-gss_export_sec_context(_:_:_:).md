

- GSS
-  gss_export_sec_context(\_:\_:\_:) 

Function

# gss_export_sec_context(\_:\_:\_:)

Transfers a security context to another process.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_export_sec_context(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: UnsafeMutablePointer,
    _ interprocess_token: gss_buffer_t?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context to export.

`interprocess_token`  

A buffer the function fills with a token corresponding to the context. Release the buffer storage with a call to gss_release_buffer(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Discussion

The function deactivates the context before exporting it. Use gss_import_sec_context(_:_:_:) to restore the token to a context and reactivate it. Only one instance of a given context may be active at a time.

## See Also

### Import and Export

func gss_import_sec_context(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, UnsafeMutablePointer&lt;gss_ctx_id_t?>) -> OM_uint32

Imports a security context from another process.

