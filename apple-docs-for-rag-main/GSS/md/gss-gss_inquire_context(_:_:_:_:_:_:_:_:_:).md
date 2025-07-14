

- GSS
-  gss_inquire_context(\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# gss_inquire_context(\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Returns information about a security context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_inquire_context(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: gss_ctx_id_t,
    _ src_name: UnsafeMutablePointer?,
    _ targ_name: UnsafeMutablePointer?,
    _ lifetime_rec: UnsafeMutablePointer?,
    _ mech_type: UnsafeMutablePointer?,
    _ ctx_flags: UnsafeMutablePointer?,
    _ locally_initiated: UnsafeMutablePointer?,
    _ xopen: UnsafeMutablePointer?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context to obtain information about.

`src_name`  

A pointer the function uses to return the name of the initiator. Free the name object’s memory with a call to gss_release_name(_:_:) when you are done with it. Specify `NULL` to ignore this output.

`targ_name`  

A pointer the function uses to return the name of the acceptor. Free the name object’s memory with a call to gss_release_name(_:_:) when you are done with it. Specify `NULL` to ignore this output.

`lifetime_rec`  

A pointer the function uses to return the number of seconds before the context expires, or zero if it has already expired. If the context does not support expiration, it returns GSS_C_INDEFINITE. Specify `NULL` to ignore this output.

`mech_type`  

A pointer the function uses to return the mechanism providing the context. Do not release the OID object, because it is held in static memory. Specify `NULL` to ignore this output.

`ctx_flags`  

A pointer the function uses to return the flags associated with the context. See Context Services for a description of available flags. Specify NULL to ignore this output.

`locally_initiated`  

A pointer the function uses to return an indicator of the context’s point of origin. The value is zero when the function is called by context’s acceptor and non-zero otherwise. Specify NULL to ignore this output.

`xopen`  

A pointer the function uses to return an indicator of the context’s current state. The value is non-zero when the context if fully established and zero otherwise. Specify NULL to ignore this output.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Discussion

The context must exist but need not be fully established for the inquiry to succeed.

## See Also

### Inquiry and Limits

func gss_context_time(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, UnsafeMutablePointer&lt;OM_uint32>) -> OM_uint32

Returns the amount of time remaining before a context expires.

func gss_inquire_sec_context_by_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_OID, UnsafeMutablePointer&lt;gss_buffer_set_t>?) -> OM_uint32

Returns information about a particular part of a context.

func gss_wrap_size_limit(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_qop_t, OM_uint32, UnsafeMutablePointer&lt;OM_uint32>) -> OM_uint32

Returns the largest allowable wrap size for a given set of constraints.

