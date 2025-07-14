

- GSS
-  gss_inquire_saslname_for_mech(\_:\_:\_:\_:\_:) 

Function

# gss_inquire_saslname_for_mech(\_:\_:\_:\_:\_:)

Returns the Simple Authentication and Security Layer (SASL) protocol name for a given GSS-API mechanism.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
func gss_inquire_saslname_for_mech(
    _ minor_status: UnsafeMutablePointer,
    _ desired_mech: gss_OID,
    _ sasl_mech_name: gss_buffer_t?,
    _ mech_name: gss_buffer_t?,
    _ mech_description: gss_buffer_t?
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`desired_mech`  

The GSS-API mechanism to query.

`sasl_mech_name`  

A buffer the function fills with the SASL G2 protocol name. Release this buffer with a call to gss_release_buffer(_:_:) when you are done with it.

`mech_name`  

A buffer the function fills with a human readable version of the GSS-API protocol name. Release this buffer with a call to gss_release_buffer(_:_:) when you are done with it.

`mech_description`  

A buffer the function fills with a description of the GSS-API protocol name. Release this buffer with a call to gss_release_buffer(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success or GSS_S_BAD_MECH if the desired mechanism is unsupported. See Function Status for a complete enumeration of status outputs.

## See Also

### Queries

func gss_indicate_mechs(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Returns the list of supported underlying security mechanisms.

func gss_indicate_mechs_by_attrs(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID_set?, gss_const_OID_set?, gss_const_OID_set?, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Returns the set of mechanisms that fulfill the given criteria.

func gss_display_mech_attr(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, gss_buffer_t?, gss_buffer_t?, gss_buffer_t?) -> OM_uint32

Returns a human-readable name and description of a mechanism attribute.

func gss_inquire_attrs_for_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;gss_OID_set?>?) -> OM_uint32

Returns the supported attributes for one or all mechanisms.

func gss_inquire_mech_for_saslname(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t?, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Returns the GSS-API mechanism identifier for a given Simple Authentication and Security Layer (SASL) protocol name.

