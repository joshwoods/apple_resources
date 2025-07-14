

- GSS
-  gss_duplicate_name(\_:\_:\_:) 

Function

# gss_duplicate_name(\_:\_:\_:)

Returns a copy of an internal name.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_duplicate_name(
    _ minor_status: UnsafeMutablePointer,
    _ src_name: gss_name_t,
    _ dest_name: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`src_name`  

The name to duplicate.

`dest_name`  

A pointer the function uses to return the copied name. Release the name using a call to the gss_release_name(_:_:) function when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## See Also

### Inquiries

func gss_display_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_buffer_t, UnsafeMutablePointer&lt;gss_OID?>?) -> OM_uint32

Converts a name in the internal format to an octet string and the associated name type.

func gss_compare_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_name_t, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns a flag that indicates if two names in internal name format refer to the same entity.

func gss_inquire_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;gss_OID?>?, UnsafeMutablePointer&lt;gss_buffer_set_t?>?) -> OM_uint32

Returns information about a name.

func gss_inquire_mechs_for_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Returns a list of mechanisms that support a particular name type.

func gss_inquire_names_for_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Returns a list of name types that a given mechanism supports.

func gss_aapl_change_password(gss_name_t, gss_const_OID, CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> OM_uint32

Changes the password associated with a name.

func gss_userok(gss_name_t, UnsafePointer&lt;CChar>) -> Int32

Returns a flag that indicates if a given user is authorized.

