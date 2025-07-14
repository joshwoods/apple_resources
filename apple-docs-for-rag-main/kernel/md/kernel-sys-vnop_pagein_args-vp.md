

- Kernel
- sys
- vnop_pagein_args
-  vp 

# vp

The vnode for which to preallocate space.

## See Also

### Fields

length

Desired preallocated file length.

flags

PREALLOCATE: preallocate allocation blocks. ALLOCATECONTIG: allocate contigious space. ALLOCATEALL: allocate all requested space or no space at all. FREEREMAINDER: deallocate allocated but unfilled blocks. ALLOCATEFROMPEOF: allocate from the physical eof. ALLOCATEFROMVOL: allocate from the volume offset.

bytesallocated

Additional bytes set aside for file. Set to 0 if none are allocated OR if the file is contracted.

offset

Hint for where to find free blocks.

ctx

Context to authenticate for allocation request.

