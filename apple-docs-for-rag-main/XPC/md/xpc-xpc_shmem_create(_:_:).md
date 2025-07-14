

- XPC
-  xpc_shmem_create(\_:\_:) 

Function

# xpc_shmem_create(\_:\_:)

Creates an XPC object that represents the specified shared memory region.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_shmem_create(
    _ region: UnsafeMutableRawPointer,
    _ length: Int
) -> xpc_object_t
```

## Parameters 

`region`  

A pointer to a region of shared memory, created through a call to mmap(2) with the MAP_SHARED flag, which is to be boxed.

`length`  

The length of the region.

## Return Value

A new shared memory object.

## Discussion

This API is NOT for making a private region of memory shareable. It is to allow for already-shareable regions of memory to be boxed in an XPC object. Do not pass a region allocated with `malloc(3)` or friends to this API.

## See Also

### Shared memory objects

func xpc_shmem_map(xpc_object_t, UnsafeMutablePointer&lt;UnsafeMutableRawPointer?>) -> Int

Maps the region that the XPC shared memory object boxes into the caller’s address space.

