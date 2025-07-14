

- GSS
-  gss_aapl_change_password(\_:\_:\_:\_:) 

Function

# gss_aapl_change_password(\_:\_:\_:\_:)

Changes the password associated with a name.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
func gss_aapl_change_password(
    _ name: gss_name_t,
    _ mech: gss_const_OID,
    _ attributes: CFDictionary,
    _ error: UnsafeMutablePointer?>?
) -> OM_uint32
```

## Parameters 

`name`  

The GSS name for which you want to change the password.

`mech`  

The underlying mechanism in use. For example, use GSS_KRB5_MECHANISM for Kerberos.

`attributes`  

A dictionary that you use to specify the old and new passwords as string values. Use the keys kGSSChangePasswordOldPassword and kGSSChangePasswordNewPassword for the old and new passwords, respectively.

`error`  

A `CFErrorRef` pointer that the function sets to point at a new error object if the function call fails. Pass `NULL` to ignore this error. When an error does exist, it describes the reason for the failure, and you are responsible for releasing it with `CFRelease`.

## Return Value

A major status code set to GSS_S_COMPLETE if the call succeeds, or some other value indicating the reason for failure if not.

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

func gss_duplicate_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Returns a copy of an internal name.

func gss_userok(gss_name_t, UnsafePointer&lt;CChar>) -> Int32

Returns a flag that indicates if a given user is authorized.

