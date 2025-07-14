

- GSS
-  gss_destroy_cred(\_:\_:) 

Function

# gss_destroy_cred(\_:\_:)

Purges a credential from memory.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_destroy_cred(
    _ min_stat: UnsafeMutablePointer,
    _ cred_handle: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`min_stat`  

A pointer to the secondary status result that provides additional information in case of failure.

`cred_handle`  

The credential to eliminate from memory.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Mentioned in 

Allocating and Releasing Objects

## Discussion

This function actively purges the credential from memory and then calls gss_release_cred(_:_:) to free the memory. This is a more secure option than calling the release function directly.

## See Also

### Allocation and Deallocation

func GSSCreateCredentialFromUUID(CFUUID) -> gss_cred_id_t?

Creates a credential from a universally unique identifier.

func gss_add_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, gss_name_t?, gss_OID?, gss_cred_usage_t, OM_uint32, OM_uint32, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Adds a new credential element to an existing credential.

func gss_set_cred_option(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>?, gss_OID, gss_buffer_t?) -> OM_uint32

Changes a credential option.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

