

- GSS
- gss_buffer_set_desc_struct
-  init(count:elements:) 

Initializer

# init(count:elements:)

Initialize a new buffer set with the given buffers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
init(
    count: Int,
    elements: UnsafeMutablePointer!
)
```

## Parameters 

`count`  

The number of buffers in the `elements` array.

`elements`  

An array of buffers to be included in the new set.

## See Also

### Initialization

init()

Initialize a new, empty buffer set.

