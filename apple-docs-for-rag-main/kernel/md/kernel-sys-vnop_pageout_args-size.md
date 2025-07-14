

- Kernel
- sys
- vnop_pageout_args
-  size 

# size

Amount of data to page in (in bytes).

## See Also

### Fields

vp

The vnode for which to page in data.

pl

UPL describing pages needing to be paged in.

pl_offset

Offset in UPL at which to start placing data.

f_offset

Offset in file of data needing to be paged in.

flags

UPL-style flags: UPL_IOSYNC, UPL_NOCOMMIT, UPL_NORDAHEAD, UPL_VNODE_PAGER, UPL_MSYNC. Filesystems should generally leave it to the cluster layer to handle these flags. See the memory_object_types.h header in the kernel framework if interested.

ctx

Context to authenticate for pagein request.

