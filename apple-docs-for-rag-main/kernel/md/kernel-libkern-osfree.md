

- Kernel
- libkern
-  OSFree 

Function

# OSFree

Frees a block of memory allocated by OSMalloc.

macOS 10.4+

``` source
void OSFree(void *addr, uint32_t size, OSMallocTag tag);
```

## Parameters 

`addr`  

A pointer to the memory block to free.

`size`  

The size of the memory block to free.

`tag`  

The OSMallocTag with which `addr` was originally allocated.

## See Also

### Memory

OSMalloc

Allocates a block of memory associated with a given OSMallocTag.

OSMalloc_Tagalloc

Creates a tag for use with OSMalloc functions.

OSMalloc_Tagfree

Frees a tag used with OSMalloc functions.

OSMalloc_noblock

Allocates a block of memory associated with a given OSMallocTag, returning `NULL` if it would block.

OSMalloc_nowait

Equivalent to OSMalloc_noblock.

bzero

bzero_phys

