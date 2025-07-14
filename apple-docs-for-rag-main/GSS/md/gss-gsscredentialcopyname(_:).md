

- GSS
-  GSSCredentialCopyName(\_:) 

Function

# GSSCredentialCopyName(\_:)

Returns the name describing the credential.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
func GSSCredentialCopyName(_ cred: gss_cred_id_t) -> gss_name_t?
```

## Parameters 

`cred`  

The credential from which to get the name.

## Return Value

A GSS name for the given credential, or NULL on failure. Release this object with a call to gss_release_name(_:_:) when you are done with it.

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

func gss_pseudo_random(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_buffer_t, Int, gss_buffer_t) -> OM_uint32

Returns a pseudo-random byte stream for keying.

