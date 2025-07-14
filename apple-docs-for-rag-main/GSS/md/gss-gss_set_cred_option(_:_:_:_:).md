

- GSS
-  gss_set_cred_option(\_:\_:\_:\_:) 

Function

# gss_set_cred_option(\_:\_:\_:\_:)

Changes a credential option.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_set_cred_option(
    _ minor_status: UnsafeMutablePointer,
    _ cred_handle: UnsafeMutablePointer?,
    _ object: gss_OID,
    _ value: gss_buffer_t?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`cred_handle`  

The credential to update.

`object`  

An object identifier that indicates the characteristic of the credential that should be changed.

`value`  

The new value for the named object.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## See Also

### Allocation and Deallocation

func GSSCreateCredentialFromUUID(CFUUID) -> gss_cred_id_t?

Creates a credential from a universally unique identifier.

func gss_add_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, gss_name_t?, gss_OID?, gss_cred_usage_t, OM_uint32, OM_uint32, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Adds a new credential element to an existing credential.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

func gss_destroy_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Purges a credential from memory.

