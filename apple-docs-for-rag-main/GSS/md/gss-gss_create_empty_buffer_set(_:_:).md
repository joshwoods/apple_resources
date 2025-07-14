

- GSS
-  gss_create_empty_buffer_set(\_:\_:) 

Function

# gss_create_empty_buffer_set(\_:\_:)

Allocates an empty buffer set descriptor that you use to manage an array of buffers.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_create_empty_buffer_set(
    _ minor_status: UnsafeMutablePointer,
    _ buffer_set: UnsafeMutablePointer
) -> OM_uint32
```

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure. Typically, a failure results from an inability to allocate memory which is communicated by the minor status ENOMEM.

`buffer_set`  

A pointer to a buffer set descriptor reference. When the function successfully allocates a buffer set descriptor, it sets the reference to point at it. The descriptor itself is initialized with zero length and a `NULL` pointer.

On failure, the reference is unchanged.

## Return Value

A status code set to GSS_S_COMPLETE on success, or GSS_S_FAILURE otherwise. Inspect the `minor_status` parameter for additional information on failure.

## Mentioned in 

Allocating and Releasing Objects

## Discussion

This function allocates memory for the data structure that you use to manage an array of buffers, consisting of a length parameter and a pointer. It does not allocate memory for any actual buffers.

When you’re done with the buffer set descriptor created by this function, call gss_release_buffer_set(_:_:) to free its memory, as well as that of any buffers it contains at that time.

## See Also

### Allocation and Deallocation

func gss_add_buffer_set_member(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, UnsafeMutablePointer&lt;gss_buffer_set_t>) -> OM_uint32

Copies the contents of a buffer into a buffer set.

func gss_release_buffer(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t) -> OM_uint32

Frees the memory associated with a single buffer descriptor.

func gss_release_buffer_set(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_buffer_set_t?>) -> OM_uint32

Frees the memory associated with a buffer set descriptor and all the buffers it contains.

