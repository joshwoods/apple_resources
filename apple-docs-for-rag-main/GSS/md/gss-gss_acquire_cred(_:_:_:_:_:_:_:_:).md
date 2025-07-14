

- GSS
-  gss_acquire_cred(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# gss_acquire_cred(\_:\_:\_:\_:\_:\_:\_:\_:)

Acquires a credential for use in establishing a security context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_acquire_cred(
    _ minor_status: UnsafeMutablePointer,
    _ desired_name: gss_name_t?,
    _ time_req: OM_uint32,
    _ desired_mechs: gss_OID_set?,
    _ cred_usage: gss_cred_usage_t,
    _ output_cred_handle: UnsafeMutablePointer,
    _ actual_mechs: UnsafeMutablePointer?,
    _ time_rec: UnsafeMutablePointer?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`desired_name`  

The name of the principal whose credential should be acquired. Specify `GSS_C_NO_NAME` to get a generic credential or use gss_import_name(_:_:_:_:) to obtain a name object.

`time_req`  

The time in seconds that the credential should remain valid. Use GSS_C_INDEFINITE to indicate the maximum allowed duration.

`desired_mechs`  

The set of underlying security mechanisms to use with the credential. Use `GSS_C_NO_OID_SET` to get the default set.

`cred_usage`  

A flag that indicates how the credential will be used. Specify GSS_C_INITIATE for context initiation, GSS_C_ACCEPT for context acceptance, or GSS_C_BOTH for both.

`output_cred_handle`  

A pointer the function uses to return the credential. Release the credential’s memory with gss_release_cred(_:_:) when you are done with it.

`actual_mechs`  

A pointer the function uses to return the actual mechanisms used by the credential. Set to `NULL` to ignore this output. If you do receive a set of mechanisms, use gss_release_oid_set(_:_:) to release its memory when you are done with it.

`time_rec`  

A pointer the function uses to return the actual number of seconds for which the credential is valid. Set to `NULL` to ignore this output.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Mentioned in 

Allocating and Releasing Objects

## See Also

### Acquisition

func gss_aapl_initial_cred(gss_name_t, gss_const_OID, CFDictionary?, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> OM_uint32

Acquires a new credential using a password or certificate.

func gss_acquire_cred_with_password(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_buffer_t, OM_uint32, gss_OID_set?, gss_cred_usage_t, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Acquires a credential for use in establishing a security context using a password.

func GSSCredentialCopyUUID(gss_cred_id_t) -> Unmanaged&lt;CFUUID>?

Returns a copy of the universally unique identifier corresponding to a GSS credential.

func GSSCredentialCopyName(gss_cred_id_t) -> gss_name_t?

Returns the name describing the credential.

func gss_pseudo_random(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_buffer_t, Int, gss_buffer_t) -> OM_uint32

Returns a pseudo-random byte stream for keying.

