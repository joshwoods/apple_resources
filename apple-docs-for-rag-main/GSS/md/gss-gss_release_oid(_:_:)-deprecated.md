

- GSS
-  gss_release_oid(\_:\_:) Deprecated

Function

# gss_release_oid(\_:\_:)

Releases the memory associated with an object identifier.

visionOS 1.0–1.0Deprecated

``` source
func gss_release_oid(
    _ minor_status: UnsafeMutablePointer,
    _ oid: UnsafeMutablePointer
) -> OM_uint32
```

Deprecated

You never need to call this function. Because OIDs are generally passed around as static objects in memory, there is never a need to create your own, or to release them.

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`oid`  

The object identifier to release.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## Mentioned in 

Allocating and Releasing Objects

## See Also

### Creation and Release

func gss_create_empty_oid_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Allocates a new, empty set to hold object identifiers.

func gss_add_oid_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, UnsafeMutablePointer&lt;gss_OID_set>) -> OM_uint32

Adds an object identifier into an OID set.

func gss_release_oid_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Releases the memory associated with an OID set.

