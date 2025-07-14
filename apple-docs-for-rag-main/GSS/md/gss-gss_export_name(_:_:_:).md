

- GSS
-  gss_export_name(\_:\_:\_:) 

Function

# gss_export_name(\_:\_:\_:)

Returns a mechanism name in contiguous octet format.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_export_name(
    _ minor_status: UnsafeMutablePointer,
    _ input_name: gss_name_t,
    _ exported_name: gss_buffer_t
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`input_name`  

The mechanism name to export. You typically obtain a name in this format from either the gss_accept_sec_context(_:_:_:_:_:_:_:_:_:_:_:) or the gss_canonicalize_name(_:_:_:_:) function.

`exported_name`  

A buffer the function fills with a contiguous octet format version of the name. Release the buffer with a call to gss_release_buffer(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## See Also

### Imports and Exports

func gss_import_name(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, gss_const_OID?, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Converts a name in contiguous octet format to the internal name format.

