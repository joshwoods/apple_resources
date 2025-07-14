

- GSS
-  GSSCreateCredentialFromUUID(\_:) 

Function

# GSSCreateCredentialFromUUID(\_:)

Creates a credential from a universally unique identifier.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
func GSSCreateCredentialFromUUID(_ uuid: CFUUID) -> gss_cred_id_t?
```

## Parameters 

`uuid`  

The universally unique identifier of the credential to fetch.

## Return Value

A GSS credential for a given ``` CF``UUID ``` object if the credential exists, otherwise `NULL`. Free the credential’s memory with gss_release_cred(_:_:) when you are done with it.

## Discussion

Use this function to get the credential corresponding to a `CFUUID` object that you originally obtained using a call to GSSCredentialCopyUUID(_:).

## See Also

### Allocation and Deallocation

func gss_add_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, gss_name_t?, gss_OID?, gss_cred_usage_t, OM_uint32, OM_uint32, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Adds a new credential element to an existing credential.

func gss_set_cred_option(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>?, gss_OID, gss_buffer_t?) -> OM_uint32

Changes a credential option.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

func gss_destroy_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Purges a credential from memory.

