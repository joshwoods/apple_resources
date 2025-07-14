

- XPC
-  xpc_shmem_map(\_:\_:) 

Function

# xpc_shmem_map(\_:\_:)

Maps the region that the XPC shared memory object boxes into the caller’s address space.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_shmem_map(
    _ xshmem: xpc_object_t,
    _ region: UnsafeMutablePointer
) -> Int
```

## Parameters 

`xshmem`  

The shared memory object to be examined.

`region`  

On return, this will point to the region at which the shared memory was mapped.

## Return Value

The length of the region that was mapped. If the mapping failed, 0 is returned.

## Discussion

The resulting region must be disposed of with `munmap(2)`.

It is the responsibility of the caller to manage protections on the new region accordingly.

## See Also

### Shared memory objects

func xpc_shmem_create(UnsafeMutableRawPointer, Int) -> xpc_object_t

Creates an XPC object that represents the specified shared memory region.

