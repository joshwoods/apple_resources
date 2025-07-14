

- GSS
-  gss_inquire_cred(\_:\_:\_:\_:\_:\_:) 

Function

# gss_inquire_cred(\_:\_:\_:\_:\_:\_:)

Obtains information about a credential.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_inquire_cred(
    _ minor_status: UnsafeMutablePointer,
    _ cred_handle: gss_cred_id_t?,
    _ name_ret: UnsafeMutablePointer?,
    _ lifetime: UnsafeMutablePointer?,
    _ cred_usage: UnsafeMutablePointer?,
    _ mechanisms: UnsafeMutablePointer?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`cred_handle`  

The credential to inspect. Use GSS_C_NO_CREDENTIAL to inquire about the default initiator principal.

`name_ret`  

A pointer the function uses to return the name that the credential asserts. Use gss_release_name(_:_:) to free the name object’s memory when you are done with it. Set the parameter to `NULL` to ignore this output.

`lifetime`  

A pointer the function uses to return the number of seconds for which the credential will remain valid, or 0 if the credential is expired. For credentials that do not support expiry, the function returns GSS_C_INDEFINITE. Set to `NULL` to ignore this output.

`cred_usage`  

A pointer the function uses to return the credential usage. The value is one of GSS_C_ACCEPT, GSS_C_INITIATE, or GSS_C_BOTH. Set to `NULL` to ignore this output.

`mechanisms`  

A pointer the function uses to return the set of mechanisms that the credential supports. Use gss_release_oid_set(_:_:) to free the set’s memory when you are done with it. Set the parameter to `NULL` to ignore this output.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## See Also

### Inquiries

func gss_inquire_cred_by_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, gss_OID, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_usage_t>?) -> OM_uint32

Obtains per-mechanism information about a credential.

func gss_inquire_cred_by_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, gss_OID, UnsafeMutablePointer&lt;gss_buffer_set_t?>) -> OM_uint32

Inquires about a particular characteristic of a credential.

func GSSCredentialGetLifetime(gss_cred_id_t) -> OM_uint32

Returns the remaining time in seconds before the credential expires.

