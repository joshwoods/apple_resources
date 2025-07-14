

- GSS
-  GSSCreateError(\_:\_:\_:) 

Function

# GSSCreateError(\_:\_:\_:)

Returns an error object based on GSS-API major and minor status codes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
func GSSCreateError(
    _ mech: gss_const_OID,
    _ major_status: OM_uint32,
    _ minor_status: OM_uint32
) -> Unmanaged?
```

## Parameters 

`mech`  

The underlying mechanism in use. For example, use GSS_KRB5_MECHANISM for Kerberos. Use GSS_C_NO_OID if none is available.

`major_status`  

Major status code from a failed GSS-API function call.

`minor_status`  

Minor status code from a failed GSS-API function call.

## Return Value

A CFError instance that corresponds to the failure described by the inputs. Release the error with CFRelease when you are done with it.

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

func gss_display_status(UnsafeMutablePointer&lt;OM_uint32>, OM_uint32, Int32, gss_OID?, UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t) -> OM_uint32

Returns a human readable string for a status code.

