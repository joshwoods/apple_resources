

- GSS
-  gss_OID_set_desc_struct 

Structure

# gss_OID_set_desc_struct

The structure for an OID set descriptor that manages an array of OID descriptors.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
struct gss_OID_set_desc_struct
```

## Topics

### Instance Properties

var count: Int

The number of OID descriptors in the array.

var elements: gss_OID!

A pointer to the array of OID descriptors.

### Initialization

init()

Initialize a new, empty object identifier set.

init(count: Int, elements: gss_OID!)

Initialize a new object identifier set with the given identifiers.

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

struct gss_OID_desc_struct

The structure for an OID descriptor that exchanges object identifiers with many GSS-API functions.

typealias gss_OID_set_desc

The descriptor that manages an array of OID descriptors.

