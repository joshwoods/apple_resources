

- GSS
-  Object Identifiers 

API Collection

# Object Identifiers

Store security mechanisms, QOPs (Quality of Protection values), and name types.

## Topics

### Object IDs

typealias gss_OID

A pointer to the OID descriptor that exchanges object identifiers with many GSS-API functions.

typealias gss_OID_set

A pointer to a descriptor that manages an array of OID descriptors.

typealias gss_OID_desc

The OID descriptor that exchanges object identifiers with many GSS-API functions.

typealias gss_const_OID

A pointer to an immutable OID descriptor exchanges object identifiers with many GSS-API functions.

typealias gss_const_OID_set

A pointer to an immutable descriptor manages an array of OID descriptors.

struct gss_OID_desc_struct

The structure for an OID descriptor that exchanges object identifiers with many GSS-API functions.

typealias gss_OID_set_desc

The descriptor that manages an array of OID descriptors.

struct gss_OID_set_desc_struct

The structure for an OID set descriptor that manages an array of OID descriptors.

### Quality of Protection Constants

var GSS_C_QOP_DEFAULT: Int32

The default Quality of Protection for per-message services.

var GSS_KRB5_CONF_C_QOP_DES: Int32

The Kerberos 5 Qualty of Service 56-bit DES encryption.

var GSS_KRB5_CONF_C_QOP_DES3_KD: Int32

The Kerberos 5 Qualty of Service 168-bit DES3 encryption with key derivation.

### Creation and Release

func gss_create_empty_oid_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Allocates a new, empty set to hold object identifiers.

func gss_add_oid_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, UnsafeMutablePointer&lt;gss_OID_set>) -> OM_uint32

Adds an object identifier into an OID set.

func gss_release_oid_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID_set?>) -> OM_uint32

Releases the memory associated with an OID set.

func gss_release_oid(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Releases the memory associated with an object identifier.

Deprecated

### Conversion and Duplication

func gss_oid_to_str(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, gss_buffer_t) -> OM_uint32

Converts an OID object to a human-readable string.

func gss_test_oid_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_const_OID, gss_OID_set, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns a flag that indicates if an OID is present in an OID set.

func gss_oid_equal(gss_const_OID?, gss_const_OID?) -> Int32

Returns a flag that indicates whether two object identifiers are the same.

func gss_duplicate_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_OID, UnsafeMutablePointer&lt;gss_OID?>) -> OM_uint32

Copies an OID into a new object.

Deprecated

## See Also

### Names and Object Identifiers

Name Handling

Manage names for GSS-API principals such as a person, a machine, or an application.

