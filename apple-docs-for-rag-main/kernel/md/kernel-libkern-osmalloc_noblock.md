

- Kernel
- libkern
-  OSMalloc_noblock 

Function

# OSMalloc_noblock

Allocates a block of memory associated with a given OSMallocTag, returning `NULL` if it would block.

macOS 10.4+

``` source
void * OSMalloc_noblock(uint32_t size, OSMallocTag tag);
```

## Parameters 

`size`  

The size of the memory block to allocate.

`tag`  

The OSMallocTag under which to allocate the memory.

## Return Value

A pointer to the memory on success, `NULL` on failure or if allocation would block.

## Discussion

If `tag` was created with the `OSMT_PAGEABLE` attribute *and*` size` is a full page or larger, the allocated memory is pageable; otherwise it is wired.

This function is guaranteed not to block.

## See Also

### Memory

OSMalloc

Allocates a block of memory associated with a given OSMallocTag.

OSMalloc_Tagalloc

Creates a tag for use with OSMalloc functions.

OSMalloc_Tagfree

Frees a tag used with OSMalloc functions.

OSMalloc_nowait

Equivalent to OSMalloc_noblock.

OSFree

Frees a block of memory allocated by OSMalloc.

bzero

bzero_phys

