

- GSS
-  gss_duplicate_oid(\_:\_:\_:) Deprecated

Function

# gss_duplicate_oid(\_:\_:\_:)

Copies an OID into a new object.

visionOS 1.0–1.0Deprecated

``` source
func gss_duplicate_oid(
    _ minor_status: UnsafeMutablePointer,
    _ src_oid: gss_OID,
    _ dest_oid: UnsafeMutablePointer
) -> OM_uint32
```

Deprecated

You never need to call this function. Because OIDs are generally passed around as static objects in memory, there is never a need to create your own, or to release them.

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`src_oid`  

The OID to copy.

`dest_oid`  

A pointer the function uses to return a copy of the OID. Use gss_release_oid(_:_:) to release this object’s memory when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## Mentioned in 

Allocating and Releasing Objects

## See Also

### Conversion and Duplication

func gss_oid_to_str(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, gss_buffer_t) -> OM_uint32

Converts an OID object to a human-readable string.

func gss_test_oid_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, gss_OID_set, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns a flag that indicates if an OID is present in an OID set.

func gss_oid_equal(gss_const_OID?, gss_const_OID?) -> Int32

Returns a flag that indicates whether two object identifiers are the same.

