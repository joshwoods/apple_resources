

- GSS
-  GSSNameCreateDisplayString(\_:) 

Function

# GSSNameCreateDisplayString(\_:)

Returns a string suitable for displaying to the user from a GSS name.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+visionOS 1.0+

``` source
func GSSNameCreateDisplayString(_ name: gss_name_t) -> Unmanaged?
```

## Parameters 

`name`  

The GSS name from which to get the display string.

## Return Value

A `CFString` object that contains a string suitable for display to the user. Use `CFRelease` to free this object’s memory when you are done with it.

## Discussion

Do not use the result of this function call to verify ACL subjects.

## See Also

### Creation and Destruction

typealias gss_name_t

A pointer to an opaque type that you use to communicate name objects with GSS-API functions.

typealias gss_const_name_t

A pointer to an immutable version of the opaque descriptor used to exchange name objects with GSS-API functions.

func gss_canonicalize_name(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_OID, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Converts an internal name into a mechanism name.

func GSSCreateName(CFTypeRef, gss_const_OID, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> gss_name_t?

Returns a GSS name given a buffer and a type.

func gss_release_name(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_name_t?>) -> OM_uint32

Frees the resources associated with a name object.

