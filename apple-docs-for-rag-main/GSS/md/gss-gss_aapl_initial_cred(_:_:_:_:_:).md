

- GSS
-  gss_aapl_initial_cred(\_:\_:\_:\_:\_:) 

Function

# gss_aapl_initial_cred(\_:\_:\_:\_:\_:)

Acquires a new credential using a password or certificate.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_aapl_initial_cred(
    _ desired_name: gss_name_t,
    _ desired_mech: gss_const_OID,
    _ attributes: CFDictionary?,
    _ output_cred_handle: UnsafeMutablePointer,
    _ error: UnsafeMutablePointer?>?
) -> OM_uint32
```

## Parameters 

`desired_name`  

The name to use to acquire the credential. Import the name using gss_import_name(_:_:_:_:). Ensure that the mechanism specified by the `desired_mech` parameter supports the name type.

`desired_mech`  

The mechanism to use to acquire the credential, for example GSS_KRB5_MECHANISM or GSS_NTLM_MECHANISM. Use gss_indicate_mechs(_:_:) to get a complete list of supported mechanisms.

`attributes`  

A dictionary that includes either the key kGSSICPassword to specify a password or kGSSICCertificate to name a certificate for use in acquiring the credential. It may also contain any of the other keys listed in Initial Credential Keys in Credential Management to optionally condition the operation.

`output_cred_handle`  

A credential pointer that the function sets to point at the new credential on success, or sets to GSS_C_NO_CREDENTIAL on failure. Use gss_release_cred(_:_:) or gss_destroy_cred(_:_:) to release the credential’s memory when you are done with it.

`error`  

An error pointer that the function sets to point at a new error object if the function call fails. Pass `NULL` to ignore this error. When an error does exist, it describes the reason for the failure, and you are responsible for releasing it with `CFRelease`.

## Return Value

A status code set to GSS_S_COMPLETE if the call succeeds, or some other value indicating the reason for failure if not.

## Discussion

Don’t call this function on a UI update thread because it may block on network activity.

## See Also

### Acquisition

func gss_acquire_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t?, OM_uint32, gss_OID_set?, gss_cred_usage_t, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Acquires a credential for use in establishing a security context.

func gss_acquire_cred_with_password(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_buffer_t, OM_uint32, gss_OID_set?, gss_cred_usage_t, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Acquires a credential for use in establishing a security context using a password.

func GSSCredentialCopyUUID(gss_cred_id_t) -> Unmanaged&lt;CFUUID>?

Returns a copy of the universally unique identifier corresponding to a GSS credential.

func GSSCredentialCopyName(gss_cred_id_t) -> gss_name_t?

Returns the name describing the credential.

func gss_pseudo_random(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_buffer_t, Int, gss_buffer_t) -> OM_uint32

Returns a pseudo-random byte stream for keying.

