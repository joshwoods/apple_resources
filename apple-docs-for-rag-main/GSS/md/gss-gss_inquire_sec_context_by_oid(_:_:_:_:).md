

- GSS
-  gss_inquire_sec_context_by_oid(\_:\_:\_:\_:) 

Function

# gss_inquire_sec_context_by_oid(\_:\_:\_:\_:)

Returns information about a particular part of a context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_inquire_sec_context_by_oid(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: gss_ctx_id_t,
    _ desired_object: gss_OID,
    _ data_set: UnsafeMutablePointer?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context to inquire about.

`desired_object`  

The object identifier naming the aspect of the context to examine.

`data_set`  

A pointer to a buffer set that includes the reference objects. Free this buffer set with gss_release_buffer_set(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## See Also

### Inquiry and Limits

func gss_context_time(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, UnsafeMutablePointer&lt;OM_uint32>) -> OM_uint32

Returns the amount of time remaining before a context expires.

func gss_inquire_context(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_OID?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;Int32>?) -> OM_uint32

Returns information about a security context.

func gss_wrap_size_limit(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_qop_t, OM_uint32, UnsafeMutablePointer&lt;OM_uint32>) -> OM_uint32

Returns the largest allowable wrap size for a given set of constraints.

