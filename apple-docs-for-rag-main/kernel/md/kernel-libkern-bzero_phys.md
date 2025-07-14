

- Kernel
- libkern
-  bzero_phys 

Function

# bzero_phys

macOS 10.3+

``` source
void bzero_phys(addr64_t phys_address, uint32_t length);
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

OSMalloc_nowait

Equivalent to OSMalloc_noblock.

OSFree

Frees a block of memory allocated by OSMalloc.

bzero

