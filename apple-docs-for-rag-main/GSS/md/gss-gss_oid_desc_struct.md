

- GSS
-  gss_OID_desc_struct 

Structure

# gss_OID_desc_struct

The structure for an OID descriptor that exchanges object identifiers with many GSS-API functions.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
struct gss_OID_desc_struct
```

## Topics

### Instance Properties

var elements: UnsafeMutableRawPointer!

A pointer to the octets that make up the object identifier.

var length: OM_uint32

The number of octets in the object identifier.

### Initialization

init()

Initialize a new, empty object identifier.

init(length: OM_uint32, elements: UnsafeMutableRawPointer!)

Initialize a new object identifier with the given array of octets.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

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

typealias gss_OID_set_desc

The descriptor that manages an array of OID descriptors.

struct gss_OID_set_desc_struct

The structure for an OID set descriptor that manages an array of OID descriptors.

