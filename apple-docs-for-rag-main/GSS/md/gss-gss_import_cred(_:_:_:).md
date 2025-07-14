

- GSS
-  gss_import_cred(\_:\_:\_:) 

Function

# gss_import_cred(\_:\_:\_:)

Imports a credential from a token.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_import_cred(
    _ minor_status: UnsafeMutablePointer,
    _ token: gss_buffer_t,
    _ cred_handle: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`token`  

The token containing the data that represents the credential.

`cred_handle`  

A pointer to a credential that the function uses to return the credential. Free the credential’s memory with gss_release_cred(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Discussion

You can import a credential from a token created with gss_export_cred(_:_:_:).

## See Also

### Import and Export

func gss_export_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, gss_buffer_t) -> OM_uint32

Exports a credential to a token.

