

- GSS
-  GSSCredentialGetLifetime(\_:) 

Function

# GSSCredentialGetLifetime(\_:)

Returns the remaining time in seconds before the credential expires.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
func GSSCredentialGetLifetime(_ cred: gss_cred_id_t) -> OM_uint32
```

## Parameters 

`cred`  

The credential to inspect.

## Return Value

The time in seconds that the credential has before it expires. The time is 0 if the call fails, or GSS_C_INDEFINITE if the credential never expires.

## See Also

### Inquiries

func gss_inquire_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_usage_t>?, UnsafeMutablePointer&lt;gss_OID_set?>?) -> OM_uint32

Obtains information about a credential.

func gss_inquire_cred_by_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, gss_OID, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_usage_t>?) -> OM_uint32

Obtains per-mechanism information about a credential.

func gss_inquire_cred_by_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, gss_OID, UnsafeMutablePointer&lt;gss_buffer_set_t?>) -> OM_uint32

Inquires about a particular characteristic of a credential.

