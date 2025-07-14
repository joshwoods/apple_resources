

- Kernel
- libkern
-  OSMalloc 

Function

# OSMalloc

Allocates a block of memory associated with a given OSMallocTag.

macOS 10.4+

``` source
void * OSMalloc(uint32_t size, OSMallocTag tag);
```

## Parameters 

`size`  

The size of the memory block to allocate.

`tag`  

The OSMallocTag under which to allocate the memory.

## Return Value

A pointer to the memory on success, `NULL` on failure.

## Discussion

If `tag` was created with the `OSMT_PAGEABLE` attribute *and*` size` is a full page or larger, the allocated memory is pageable; otherwise it is wired.

## See Also

### Memory

OSMalloc_Tagalloc

Creates a tag for use with OSMalloc functions.

OSMalloc_Tagfree

Frees a tag used with OSMalloc functions.

OSMalloc_noblock

Allocates a block of memory associated with a given OSMallocTag, returning `NULL` if it would block.

OSMalloc_nowait

Equivalent to OSMalloc_noblock.

OSFree

Frees a block of memory allocated by OSMalloc.

bzero

bzero_phys

