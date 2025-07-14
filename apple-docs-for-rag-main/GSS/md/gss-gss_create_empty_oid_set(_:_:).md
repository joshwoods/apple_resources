

- GSS
-  gss_create_empty_oid_set(\_:\_:) 

Function

# gss_create_empty_oid_set(\_:\_:)

Allocates a new, empty set to hold object identifiers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_create_empty_oid_set(
    _ minor_status: UnsafeMutablePointer,
    _ oid_set: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`oid_set`  

A pointer that the function uses to return the new set.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## Discussion

Use gss_add_oid_set_member(_:_:_:) to add items to your newly created set. Use gss_release_oid_set(_:_:) to free the memory associated with the set when you’re done with it.

## See Also

### Creation and Release

func gss_add_oid_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, UnsafeMutablePointer&lt;gss_OID_set>) -> OM_uint32

Adds an object identifier into an OID set.

func gss_release_oid_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Releases the memory associated with an OID set.

func gss_release_oid(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Releases the memory associated with an object identifier.

Deprecated

