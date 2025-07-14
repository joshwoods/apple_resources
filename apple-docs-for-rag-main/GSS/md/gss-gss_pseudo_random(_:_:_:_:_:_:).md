

- GSS
-  gss_pseudo_random(\_:\_:\_:\_:\_:\_:) 

Function

# gss_pseudo_random(\_:\_:\_:\_:\_:\_:)

Returns a pseudo-random byte stream for keying.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_pseudo_random(
    _ minor_status: UnsafeMutablePointer,
    _ context: gss_ctx_id_t,
    _ prf_key: Int32,
    _ prf_in: gss_buffer_t,
    _ desired_output_len: Int,
    _ prf_out: gss_buffer_t
) -> OM_uint32
```

## See Also

### Acquisition

func gss_aapl_initial_cred(gss_name_t, gss_const_OID, CFDictionary?, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> OM_uint32

Acquires a new credential using a password or certificate.

func gss_acquire_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t?, OM_uint32, gss_OID_set?, gss_cred_usage_t, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Acquires a credential for use in establishing a security context.

func gss_acquire_cred_with_password(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_buffer_t, OM_uint32, gss_OID_set?, gss_cred_usage_t, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Acquires a credential for use in establishing a security context using a password.

func GSSCredentialCopyUUID(gss_cred_id_t) -> Unmanaged&lt;CFUUID>?

Returns a copy of the universally unique identifier corresponding to a GSS credential.

func GSSCredentialCopyName(gss_cred_id_t) -> gss_name_t?

Returns the name describing the credential.

