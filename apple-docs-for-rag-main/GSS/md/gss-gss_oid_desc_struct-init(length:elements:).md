

- GSS
- gss_OID_desc_struct
-  init(length:elements:) 

Initializer

# init(length:elements:)

Initialize a new object identifier with the given array of octets.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
init(
    length: OM_uint32,
    elements: UnsafeMutableRawPointer!
)
```

## Parameters 

`length`  

The number of octets in the `elements` array.

`elements`  

A pointer to the beginning of an array of octets of the specified length that represent the object identifier.

## See Also

### Initialization

init()

Initialize a new, empty object identifier.

