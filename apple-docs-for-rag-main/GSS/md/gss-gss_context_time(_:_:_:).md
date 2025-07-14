

- GSS
-  gss_context_time(\_:\_:\_:) 

Function

# gss_context_time(\_:\_:\_:)

Returns the amount of time remaining before a context expires.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_context_time(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: gss_ctx_id_t,
    _ time_rec: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context to examine.

`time_rec`  

A pointer the function uses to return the number of seconds for which the context is valid. Returns 0 if the context is already expired.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## See Also

### Inquiry and Limits

func gss_inquire_context(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_OID?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;Int32>?) -> OM_uint32

Returns information about a security context.

func gss_inquire_sec_context_by_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_OID, UnsafeMutablePointer&lt;gss_buffer_set_t>?) -> OM_uint32

Returns information about a particular part of a context.

func gss_wrap_size_limit(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_qop_t, OM_uint32, UnsafeMutablePointer&lt;OM_uint32>) -> OM_uint32

Returns the largest allowable wrap size for a given set of constraints.

