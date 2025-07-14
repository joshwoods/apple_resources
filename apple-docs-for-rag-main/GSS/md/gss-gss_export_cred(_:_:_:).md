

- GSS
-  gss_export_cred(\_:\_:\_:) 

Function

# gss_export_cred(\_:\_:\_:)

Exports a credential to a token.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_export_cred(
    _ minor_status: UnsafeMutablePointer,
    _ cred_handle: gss_cred_id_t,
    _ token: gss_buffer_t
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`cred_handle`  

The credential that you want to export.

`token`  

A buffer representing a token that the function fills with data that represents the credential. Anything in the buffer from before the call, is discarded, even if export fails.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a description of other status outputs.

## Discussion

You can recover the credential exported this way using gss_import_cred(_:_:_:).

## See Also

### Import and Export

func gss_import_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Imports a credential from a token.

