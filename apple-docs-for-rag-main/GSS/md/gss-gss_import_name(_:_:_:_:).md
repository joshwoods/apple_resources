

- GSS
-  gss_import_name(\_:\_:\_:\_:) 

Function

# gss_import_name(\_:\_:\_:\_:)

Converts a name in contiguous octet format to the internal name format.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_import_name(
    _ minor_status: UnsafeMutablePointer,
    _ input_name_buffer: gss_buffer_t,
    _ input_name_type: gss_const_OID?,
    _ output_name: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`input_name_buffer`  

A buffer holding the octets that represent the name to import.

`input_name_type`  

An object identifier that specifies the name type. Use GSS_C_NO_OID to request the default for the mechanism.

`output_name`  

A pointer the function uses to return the imported name. Release this buffer with a call to gss_release_name(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## Discussion

Use this function to reverse the import procedure carried out with the gss_display_name(_:_:_:_:) function.

## See Also

### Imports and Exports

func gss_export_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_buffer_t) -> OM_uint32

Returns a mechanism name in contiguous octet format.

