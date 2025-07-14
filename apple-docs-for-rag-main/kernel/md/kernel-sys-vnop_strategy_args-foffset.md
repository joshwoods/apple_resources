

- Kernel
- sys
- vnop_strategy_args
-  foffset 

# foffset

Offset (in bytes) at which region starts.

## See Also

### Fields

vp

The vnode for which to get on-disk information.

size

Size of region.

bpn

Destination for physical block number at which region begins on disk.

run

Destination for number of bytes which can be found contiguously on-disk before first discontinuity.

poff

Currently unused.

flags

VNODE_READ: request is for a read. VNODE_WRITE: request is for a write.

ctx

Context to authenticate for blockmap request; currently often set to NULL.

