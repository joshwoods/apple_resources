

- GSS
-  gss_const_name_t 

Type Alias

# gss_const_name_t

A pointer to an immutable version of the opaque descriptor used to exchange name objects with GSS-API functions.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
typealias gss_const_name_t = OpaquePointer
```

## See Also

### Creation and Destruction

typealias gss_name_t

A pointer to an opaque type that you use to communicate name objects with GSS-API functions.

func gss_canonicalize_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_OID, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Converts an internal name into a mechanism name.

func GSSNameCreateDisplayString(gss_name_t) -> Unmanaged&lt;CFString>?

Returns a string suitable for displaying to the user from a GSS name.

func GSSCreateName(CFTypeRef, gss_const_OID, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> gss_name_t?

Returns a GSS name given a buffer and a type.

func gss_release_name(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Frees the resources associated with a name object.

