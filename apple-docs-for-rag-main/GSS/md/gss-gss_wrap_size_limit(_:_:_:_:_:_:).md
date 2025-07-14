

- GSS
-  gss_wrap_size_limit(\_:\_:\_:\_:\_:\_:) 

Function

# gss_wrap_size_limit(\_:\_:\_:\_:\_:\_:)

Returns the largest allowable wrap size for a given set of constraints.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_wrap_size_limit(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: gss_ctx_id_t,
    _ conf_req_flag: Int32,
    _ qop_req: gss_qop_t,
    _ req_output_size: OM_uint32,
    _ max_input_size: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context used to transmit the data.

`conf_req_flag`  

A flag that you set to a non-zero value to indicate that wrapping function will apply confidentiality in addition to integrity protection or zero if only integrity protection is required.

`qop_req`  

The required quality of protection. See Object Identifiers for possible values.

`req_output_size`  

The maximum allowable output token size from the gss_wrap(_:_:_:_:_:_:_:) function.

`max_input_size`  

A pointer the function uses to return the maximum input size.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## See Also

### Inquiry and Limits

func gss_context_time(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, UnsafeMutablePointer&lt;OM_uint32>) -> OM_uint32

Returns the amount of time remaining before a context expires.

func gss_inquire_context(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_OID?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;Int32>?) -> OM_uint32

Returns information about a security context.

func gss_inquire_sec_context_by_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_OID, UnsafeMutablePointer&lt;gss_buffer_set_t>?) -> OM_uint32

Returns information about a particular part of a context.

