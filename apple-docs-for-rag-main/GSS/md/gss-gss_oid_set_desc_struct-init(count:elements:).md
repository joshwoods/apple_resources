

- GSS
- gss_OID_set_desc_struct
-  init(count:elements:) 

Initializer

# init(count:elements:)

Initialize a new object identifier set with the given identifiers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
init(
    count: Int,
    elements: gss_OID!
)
```

## Parameters 

`count`  

The number of object identifiers in the `elements` array.

`elements`  

An array containing the identifiers with which to initialize the new set.

## See Also

### Initialization

init()

Initialize a new, empty object identifier set.

