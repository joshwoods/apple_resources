

- GSS
- gss_iov_buffer_desc_struct
-  init(type:buffer:) 

Initializer

# init(type:buffer:)

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
init(
    type: OM_uint32,
    buffer: gss_buffer_desc
)
```

## Parameters 

`type`  

The desired IOV buffer type.

`buffer`  

The buffer structure.

## Discussion

Initialize a new IOV buffer structure with the given configuration.

## See Also

### Initialization

init()

Initialize a new, empty IOV buffer structure.

