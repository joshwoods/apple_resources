

- GSS
-  gss_add_oid_set_member(\_:\_:\_:) 

Function

# gss_add_oid_set_member(\_:\_:\_:)

Adds an object identifier into an OID set.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_add_oid_set_member(
    _ minor_status: UnsafeMutablePointer,
    _ member_oid: gss_const_OID,
    _ oid_set: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`member_oid`  

The object identifier to be added.

`oid_set`  

A pointer to the set to which the new OID should be added. Use gss_create_empty_oid_set(_:_:) to create a new set.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## Discussion

If the OID already exists in the set, there is no action taken. Otherwise, the function adds the OID to the end of the set. Because the function adds the OID doesn’t copy it, the `member_oid` pointer must remain stable while the `oid_set` is in use.

## See Also

### Creation and Release

func gss_create_empty_oid_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Allocates a new, empty set to hold object identifiers.

func gss_release_oid_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Releases the memory associated with an OID set.

func gss_release_oid(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Releases the memory associated with an object identifier.

Deprecated

