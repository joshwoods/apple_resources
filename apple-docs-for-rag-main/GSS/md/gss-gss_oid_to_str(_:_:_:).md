

- GSS
-  gss_oid_to_str(\_:\_:\_:) 

Function

# gss_oid_to_str(\_:\_:\_:)

Converts an OID object to a human-readable string.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_oid_to_str(
    _ minor_status: UnsafeMutablePointer,
    _ oid: gss_OID,
    _ oid_str: gss_buffer_t
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`oid`  

The object identifier to be converted.

`oid_str`  

A buffer the function fills with the OID converted to a human readable string.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## See Also

### Conversion and Duplication

func gss_test_oid_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, gss_OID_set, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns a flag that indicates if an OID is present in an OID set.

func gss_oid_equal(gss_const_OID?, gss_const_OID?) -> Int32

Returns a flag that indicates whether two object identifiers are the same.

func gss_duplicate_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Copies an OID into a new object.

Deprecated

