

- GSS
-  gss_uint32 

Type Alias

# gss_uint32

A 32-bit unsigned integer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
typealias gss_uint32 = UInt32
```

## See Also

### Status and Error Creation

typealias OM_uint32

A 32-bit unsigned integer.

typealias OM_uint64

A 64-bit unsigned integer.

typealias gss_status_id_t

A pointer to a status result.

var GSS_C_MECH_CODE: Int32

A flag that indicates the status code comes from a call to an underlying mechanism, such as Kerberos.

var GSS_C_GSS_CODE: Int32

A flag that indicates the named status code comes from a GSS-API call.

var GSS_S_COMPLETE: Int32

The operation completed without error.

func gss_display_status(UnsafeMutablePointer&lt;OM_uint32>, OM_uint32, Int32, gss_OID?, UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t) -> OM_uint32

Returns a human readable string for a status code.

func GSSCreateError(gss_const_OID, OM_uint32, OM_uint32) -> Unmanaged&lt;CFError>?

Returns an error object based on GSS-API major and minor status codes.

