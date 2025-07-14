

- Kernel
- libkern
-  OSMalloc_Tagalloc 

Function

# OSMalloc_Tagalloc

Creates a tag for use with OSMalloc functions.

macOS 10.4+

``` source
OSMallocTag OSMalloc_Tagalloc(const char *name, uint32_t flags);
```

## Parameters 

`name`  

The name of the tag to create.

`flags`  

A bitmask that controls allocation behavior; see description.

## Return Value

An opaque tag to be used with OSMalloc functions for tracking memory usage.

## Discussion

OSMalloc tags can have arbitrary names of a length up to 63 characters. Calling this function twice with the same name creates two tags, which share that name.

`flags` can be the bitwise OR of the following flags:

- `OSMT_DEFAULT` - allocations are wired. This is the 'zero' bitmask value and is overridden by any other flag specified.

- `OSMT_PAGEABLE` - allocations of a full page size or greater are pageable; allocations smaller than a page are wired.

## See Also

### Memory

OSMalloc

Allocates a block of memory associated with a given OSMallocTag.

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

