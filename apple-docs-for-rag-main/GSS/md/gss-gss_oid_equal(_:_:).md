

- GSS
-  gss_oid_equal(\_:\_:) 

Function

# gss_oid_equal(\_:\_:)

Returns a flag that indicates whether two object identifiers are the same.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_oid_equal(
    _ a: gss_const_OID?,
    _ b: gss_const_OID?
) -> Int32
```

## Parameters 

`a`  

The first object identifier to examine.

`b`  

The second object identifier to examine.

## Return Value

A non-zero value if the objects are the same, or zero if they are different.

## See Also

### Conversion and Duplication

func gss_oid_to_str(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, gss_buffer_t) -> OM_uint32

Converts an OID object to a human-readable string.

func gss_test_oid_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, gss_OID_set, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns a flag that indicates if an OID is present in an OID set.

func gss_duplicate_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Copies an OID into a new object.

Deprecated

