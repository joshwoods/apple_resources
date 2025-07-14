

- GSS
-  gss_inquire_cred_by_mech(\_:\_:\_:\_:\_:\_:\_:) 

Function

# gss_inquire_cred_by_mech(\_:\_:\_:\_:\_:\_:\_:)

Obtains per-mechanism information about a credential.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_inquire_cred_by_mech(
    _ minor_status: UnsafeMutablePointer,
    _ cred_handle: gss_cred_id_t?,
    _ mech_type: gss_OID,
    _ cred_name: UnsafeMutablePointer?,
    _ initiator_lifetime: UnsafeMutablePointer?,
    _ acceptor_lifetime: UnsafeMutablePointer?,
    _ cred_usage: UnsafeMutablePointer?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`cred_handle`  

The credential to inspect. Use GSS_C_NO_CREDENTIAL to inquire about the default initiator principal.

`mech_type`  

The mechanism for which information should be returned.

`cred_name`  

A pointer the function uses to return the name that the credential asserts. Use gss_release_name(_:_:) to free the name object’s memory when you are done with it. Set the parameter to `NULL` to ignore this output.

`initiator_lifetime`  

A pointer the function uses to return the number of seconds for which the credential will remain valid for initiating security contexts, or 0 if the credential is expired or if the credential’s usage mechanism is GSS_C_ACCEPT. For credentials that do not support expiry, the function returns GSS_C_INDEFINITE. Set to `NULL` to ignore this output.

`acceptor_lifetime`  

A pointer the function uses to return the number of seconds for which the credential will remain valid for accepting security contexts, or 0 if the credential is expired or if the credential’s usage mechanism is GSS_C_INITIATE. For credentials that do not support expiry, the function returns GSS_C_INDEFINITE. Set to `NULL` to ignore this output.

`cred_usage`  

A pointer the function uses to return the credential usage. The value is one of GSS_C_ACCEPT, GSS_C_INITIATE, or GSS_C_BOTH. Set to `NULL` to ignore this output.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## See Also

### Inquiries

func gss_inquire_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_usage_t>?, UnsafeMutablePointer&lt;gss_OID_set?>?) -> OM_uint32

Obtains information about a credential.

func gss_inquire_cred_by_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, gss_OID, UnsafeMutablePointer&lt;gss_buffer_set_t?>) -> OM_uint32

Inquires about a particular characteristic of a credential.

func GSSCredentialGetLifetime(gss_cred_id_t) -> OM_uint32

Returns the remaining time in seconds before the credential expires.

