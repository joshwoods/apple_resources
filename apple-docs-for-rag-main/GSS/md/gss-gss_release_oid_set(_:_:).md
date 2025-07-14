

- GSS
-  gss_release_oid_set(\_:\_:) 

Function

# gss_release_oid_set(\_:\_:)

Releases the memory associated with an OID set.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_release_oid_set(
    _ minor_status: UnsafeMutablePointer,
    _ set: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`set`  

The OID set to be released.

## Return Value

A status code set to GSS_S_COMPLETE on completion. See Function Status for a complete enumeration of status outputs.

## Discussion

Use this function to free the memory associated with an OID set that you created with gss_create_empty_oid_set(_:_:), or that was created on your behalf this way. The contents of the set don’t need to be freed individually. OIDs are typically static objects that don’t require memory management.

## See Also

### Creation and Release

func gss_create_empty_oid_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Allocates a new, empty set to hold object identifiers.

func gss_add_oid_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, UnsafeMutablePointer&lt;gss_OID_set>) -> OM_uint32

Adds an object identifier into an OID set.

func gss_release_oid(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Releases the memory associated with an object identifier.

Deprecated

