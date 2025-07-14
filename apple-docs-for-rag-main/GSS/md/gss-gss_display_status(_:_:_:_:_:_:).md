

- GSS
-  gss_display_status(\_:\_:\_:\_:\_:\_:) 

Function

# gss_display_status(\_:\_:\_:\_:\_:\_:)

Returns a human readable string for a status code.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_display_status(
    _ minor_status: UnsafeMutablePointer,
    _ status_value: OM_uint32,
    _ status_type: Int32,
    _ mech_type: gss_OID?,
    _ message_content: UnsafeMutablePointer,
    _ status_string: gss_buffer_t
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`status_value`  

The status to be examined.

`status_type`  

The kind of status to be examined. Set to GSS_C_GSS_CODE for a GSS status code, or to GSS_C_MECH_CODE for a mechanism status code.

`mech_type`  

The mechanism for which to interpret the status value. Set to GSS_C_NO_OID to indicate the system default.

`message_content`  

A pointer the function uses to return a context that is currently always set to zero.

`status_string`  

A buffer the function fills with the human readable string corresponding to the status code. Release this buffer with a call to gss_release_buffer(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## See Also

### Status and Error Creation

typealias OM_uint32

A 32-bit unsigned integer.

typealias OM_uint64

A 64-bit unsigned integer.

typealias gss_uint32

A 32-bit unsigned integer.

typealias gss_status_id_t

A pointer to a status result.

var GSS_C_MECH_CODE: Int32

A flag that indicates the status code comes from a call to an underlying mechanism, such as Kerberos.

var GSS_C_GSS_CODE: Int32

A flag that indicates the named status code comes from a GSS-API call.

var GSS_S_COMPLETE: Int32

The operation completed without error.

func GSSCreateError(gss_const_OID, OM_uint32, OM_uint32) -> Unmanaged&lt;CFError>?

Returns an error object based on GSS-API major and minor status codes.

