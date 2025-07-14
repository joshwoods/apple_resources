

- GSS
-  Name Handling 

API Collection

# Name Handling

Manage names for GSS-API principals such as a person, a machine, or an application.

## Topics

### Creation and Destruction

typealias gss_name_t

A pointer to an opaque type that you use to communicate name objects with GSS-API functions.

typealias gss_const_name_t

A pointer to an immutable version of the opaque descriptor used to exchange name objects with GSS-API functions.

func gss_canonicalize_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_OID, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Converts an internal name into a mechanism name.

func GSSNameCreateDisplayString(gss_name_t) -> Unmanaged&lt;CFString>?

Returns a string suitable for displaying to the user from a GSS name.

func GSSCreateName(CFTypeRef, gss_const_OID, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> gss_name_t?

Returns a GSS name given a buffer and a type.

func gss_release_name(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Frees the resources associated with a name object.

### Inquiries

Create, compare, and examine names, the objects used to identify entities.

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

func gss_aapl_change_password(gss_name_t, gss_const_OID, CFDictionary, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> OM_uint32

Changes the password associated with a name.

func gss_userok(gss_name_t, UnsafePointer&lt;CChar>) -> Int32

Returns a flag that indicates if a given user is authorized.

### Imports and Exports

func gss_export_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_buffer_t) -> OM_uint32

Returns a mechanism name in contiguous octet format.

func gss_import_name(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, gss_const_OID?, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Converts a name in contiguous octet format to the internal name format.

## See Also

### Names and Object Identifiers

Object Identifiers

Store security mechanisms, QOPs (Quality of Protection values), and name types.

