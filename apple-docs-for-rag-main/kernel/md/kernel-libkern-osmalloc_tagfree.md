

- Kernel
- libkern
-  OSMalloc_Tagfree 

Function

# OSMalloc_Tagfree

Frees a tag used with OSMalloc functions.

macOS 10.4+

``` source
void OSMalloc_Tagfree(OSMallocTag tag);
```

## Parameters 

`tag`  

The OSMallocTag to free.

## Discussion

OSMalloc tags must not be freed while any memory blocks allocated with them still exist. Any OSMalloc function called on those blocks will result in a panic.

## See Also

### Memory

OSMalloc

Allocates a block of memory associated with a given OSMallocTag.

OSMalloc_Tagalloc

Creates a tag for use with OSMalloc functions.

OSMalloc_noblock

Allocates a block of memory associated with a given OSMallocTag, returning `NULL` if it would block.

OSMalloc_nowait

Equivalent to OSMalloc_noblock.

OSFree

Frees a block of memory allocated by OSMalloc.

bzero

bzero_phys

