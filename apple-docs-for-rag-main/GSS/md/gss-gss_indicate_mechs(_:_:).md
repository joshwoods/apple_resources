

- GSS
-  gss_indicate_mechs(\_:\_:) 

Function

# gss_indicate_mechs(\_:\_:)

Returns the list of supported underlying security mechanisms.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_indicate_mechs(
    _ minor_status: UnsafeMutablePointer,
    _ mech_set: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`mech_set`  

A pointer the function uses to output the available set of mechanism identifiers. Release the set with a call to gss_release_oid_set(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on completion.

## See Also

### Queries

func gss_indicate_mechs_by_attrs(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID_set?, gss_const_OID_set?, gss_const_OID_set?, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Returns the set of mechanisms that fulfill the given criteria.

func gss_display_mech_attr(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, gss_buffer_t?, gss_buffer_t?, gss_buffer_t?) -> OM_uint32

Returns a human-readable name and description of a mechanism attribute.

func gss_inquire_attrs_for_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;gss_OID_set?>?) -> OM_uint32

Returns the supported attributes for one or all mechanisms.

func gss_inquire_mech_for_saslname(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t?, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Returns the GSS-API mechanism identifier for a given Simple Authentication and Security Layer (SASL) protocol name.

func gss_inquire_saslname_for_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, gss_buffer_t?, gss_buffer_t?, gss_buffer_t?) -> OM_uint32

Returns the Simple Authentication and Security Layer (SASL) protocol name for a given GSS-API mechanism.

