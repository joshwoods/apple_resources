

- GSS
-  gss_import_sec_context(\_:\_:\_:) 

Function

# gss_import_sec_context(\_:\_:\_:)

Imports a security context from another process.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_import_sec_context(
    _ minor_status: UnsafeMutablePointer,
    _ interprocess_token: gss_buffer_t,
    _ context_handle: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`interprocess_token`  

The token created by a call to gss_export_sec_context(_:_:_:).

`context_handle`  

A pointer the function uses to return the imported context. Release the context with the gss_delete_sec_context(_:_:_:) function when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Discussion

You can import an interprocess token only once. After you have imported it, release the token’s buffer using a call to gss_release_buffer(_:_:).

## See Also

### Import and Export

func gss_export_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_buffer_t?) -> OM_uint32

Transfers a security context to another process.

