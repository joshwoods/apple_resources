

- GSS
-  gss_inquire_cred_by_oid(\_:\_:\_:\_:) 

Function

# gss_inquire_cred_by_oid(\_:\_:\_:\_:)

Inquires about a particular characteristic of a credential.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_inquire_cred_by_oid(
    _ minor_status: UnsafeMutablePointer,
    _ cred_handle: gss_cred_id_t,
    _ desired_object: gss_OID,
    _ data_set: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`cred_handle`  

The credential to inquire about.

`desired_object`  

The object identifier of the characteristic of the credential to return.

`data_set`  

A pointer the function uses to return a set of buffers that contain the results across all of the credential’s mechanisms. If the desired object is not found, this is set to GSS_C_NO_BUFFER_SET. Otherwise, call gss_release_buffer_set(_:_:) to free the memory of this object when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## See Also

### Inquiries

func gss_inquire_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_usage_t>?, UnsafeMutablePointer&lt;gss_OID_set?>?) -> OM_uint32

Obtains information about a credential.

func gss_inquire_cred_by_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, gss_OID, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_usage_t>?) -> OM_uint32

Obtains per-mechanism information about a credential.

func GSSCredentialGetLifetime(gss_cred_id_t) -> OM_uint32

Returns the remaining time in seconds before the credential expires.

