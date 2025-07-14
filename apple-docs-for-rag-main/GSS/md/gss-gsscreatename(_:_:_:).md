

- GSS
-  GSSCreateName(\_:\_:\_:) 

Function

# GSSCreateName(\_:\_:\_:)

Returns a GSS name given a buffer and a type.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
func GSSCreateName(
    _ name: CFTypeRef,
    _ name_type: gss_const_OID,
    _ error: UnsafeMutablePointer?>?
) -> gss_name_t?
```

## Parameters 

`name`  

A name buffer describing the credential. The buffer is either a `CFDataRef` or a `CFStringRef` containing the name.

`name_type`  

An OID name type constant, such as GSS_C_NT_USER_NAME.

`error`  

A `CFErrorRef` pointer that the function sets to point at a new error object if the function call fails, or `NULL` to ignore the error. If the error exists, it describes the reason for the failure, and you are responsible for releasing it with `CFRelease`.

## Return Value

A GSS name for the given buffer and type, or `NULL` on failure. Release this object with a call to gss_release_name(_:_:) when you are done with it.

## See Also

### Creation and Destruction

typealias gss_name_t

A pointer to an opaque type that you use to communicate name objects with GSS-API functions.

typealias gss_const_name_t

A pointer to an immutable version of the opaque descriptor used to exchange name objects with GSS-API functions.

func gss_canonicalize_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_OID, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Converts an internal name into a mechanism name.

func GSSNameCreateDisplayString(gss_name_t) -> Unmanaged&lt;CFString>?

Returns a string suitable for displaying to the user from a GSS name.

func gss_release_name(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Frees the resources associated with a name object.

