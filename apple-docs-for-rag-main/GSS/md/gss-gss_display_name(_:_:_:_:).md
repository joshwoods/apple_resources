

- GSS
-  gss_display_name(\_:\_:\_:\_:) 

Function

# gss_display_name(\_:\_:\_:\_:)

Converts a name in the internal format to an octet string and the associated name type.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_display_name(
    _ minor_status: UnsafeMutablePointer,
    _ input_name: gss_name_t,
    _ output_name_buffer: gss_buffer_t,
    _ output_name_type: UnsafeMutablePointer?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`input_name`  

The name in internal format to be converted.

`output_name_buffer`  

A buffer the function fills with the octet string that corresponds to the name. Release this buffer with a call to gss_release_buffer(_:_:) when you are done with it.

`output_name_type`  

A pointer the function uses to return an object identifier that indicates the name type.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## Discussion

Use this function to reverse the import procedure carried out with the gss_import_name(_:_:_:_:) function.

## See Also

### Inquiries

func gss_compare_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_name_t, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns a flag that indicates if two names in internal name format refer to the same entity.

func gss_inquire_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;gss_OID?>?, UnsafeMutablePointer&lt;gss_buffer_set_t?>?) -> OM_uint32

Returns information about a name.

func gss_inquire_mechs_for_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Returns a list of mechanisms that support a particular name type.

func gss_inquire_names_for_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Returns a list of name types that a given mechanism supports.

func gss_duplicate_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Returns a copy of an internal name.

func gss_aapl_change_password(gss_name_t, gss_const_OID, CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> OM_uint32

Changes the password associated with a name.

func gss_userok(gss_name_t, UnsafePointer&lt;CChar>) -> Int32

Returns a flag that indicates if a given user is authorized.

