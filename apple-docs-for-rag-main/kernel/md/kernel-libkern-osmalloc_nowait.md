

- Kernel
- libkern
-  OSMalloc_nowait 

Function

# OSMalloc_nowait

Equivalent to OSMalloc_noblock.

macOS 10.4+

``` source
void * OSMalloc_nowait(uint32_t size, OSMallocTag tag);
```

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

OSFree

Frees a block of memory allocated by OSMalloc.

bzero

bzero_phys

