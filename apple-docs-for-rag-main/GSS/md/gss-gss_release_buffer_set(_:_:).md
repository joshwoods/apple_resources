

- GSS
-  gss_release_buffer_set(\_:\_:) 

Function

# gss_release_buffer_set(\_:\_:)

Frees the memory associated with a buffer set descriptor and all the buffers it contains.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_release_buffer_set(
    _ minor_status: UnsafeMutablePointer,
    _ buffer_set: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`buffer_set`  

A pointer to the buffer set descriptor reference that you want to free.

## Return Value

A status code set to GSS_S_COMPLETE on completion.

## Mentioned in 

Allocating and Releasing Objects

## Discussion

This call frees the memory of all of the buffers that the buffer set contains, as well as the buffer set descriptor itself. Use this function when you’re done with a buffer set that you created with gss_create_empty_buffer_set(_:_:), or created on your behalf by gss_add_buffer_set_member(_:_:_:).

## See Also

### Allocation and Deallocation

func gss_create_empty_buffer_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_buffer_set_t?>) -> OM_uint32

Allocates an empty buffer set descriptor that you use to manage an array of buffers.

func gss_add_buffer_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, UnsafeMutablePointer&lt;gss_buffer_set_t>) -> OM_uint32

Copies the contents of a buffer into a buffer set.

func gss_release_buffer(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t) -> OM_uint32

Frees the memory associated with a single buffer descriptor.

