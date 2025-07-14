

- GSS
-  gss_release_name(\_:\_:) 

Function

# gss_release_name(\_:\_:)

Frees the resources associated with a name object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_release_name(
    _ minor_status: UnsafeMutablePointer,
    _ input_name: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`input_name`  

A pointer to the name that should be freed. The name is set to GSS_C_NO_NAME when the function returns successfully.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

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

func GSSCreateName(CFTypeRef, gss_const_OID, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> gss_name_t?

Returns a GSS name given a buffer and a type.

