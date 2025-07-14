

- Kernel
- sys
- vnop_pageout_args
-  ctx 

# ctx

Context to authenticate for pagein request.

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

size

Amount of data to page in (in bytes).

flags

UPL-style flags: UPL_IOSYNC, UPL_NOCOMMIT, UPL_NORDAHEAD, UPL_VNODE_PAGER, UPL_MSYNC. Filesystems should generally leave it to the cluster layer to handle these flags. See the memory_object_types.h header in the kernel framework if interested.

