

- GSS
-  gss_test_oid_set_member(\_:\_:\_:\_:) 

Function

# gss_test_oid_set_member(\_:\_:\_:\_:)

Returns a flag that indicates if an OID is present in an OID set.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_test_oid_set_member(
    _ minor_status: UnsafeMutablePointer,
    _ member: gss_const_OID,
    _ set: gss_OID_set,
    _ present: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`member`  

The OID to search for.

`set`  

The set of OIDs to search in.

`present`  

A pointer that the function uses to indicate whether or not the member is present in the set. The value is non-zero if the member is present, and zero otherwise.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## See Also

### Conversion and Duplication

func gss_oid_to_str(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, gss_buffer_t) -> OM_uint32

Converts an OID object to a human-readable string.

func gss_oid_equal(gss_const_OID?, gss_const_OID?) -> Int32

Returns a flag that indicates whether two object identifiers are the same.

func gss_duplicate_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Copies an OID into a new object.

Deprecated

