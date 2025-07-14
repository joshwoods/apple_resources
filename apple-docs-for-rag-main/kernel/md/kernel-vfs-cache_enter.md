

- Kernel
- vfs
-  cache_enter 

Function

# cache_enter

Add a (name,vnode) entry to the VFS namecache.

macOS 10.4+

``` source
void cache_enter(vnode_t dvp, vnode_t vp, struct componentname *cnp);
```

## Parameters 

`dvp`  

Directory in which file lives.

`vp`  

File to add to cache. A non-NULL vp is stored for rapid access; a NULL vp indicates that there is no such file in the directory and speeds future failed lookups.

`cnp`  

Various data about lookup, e.g. filename and intended operation.

## Return Value

void.

## Discussion

Generally used to add a cache entry after a successful filesystem-level lookup or to add a negative entry after one which did not find its target.

## See Also

### Support

nop_access

nop_advlock

nop_allocate

nop_blktooff

nop_blockmap

nop_bwrite

nop_close

nop_copyfile

nop_create

nop_exchange

nop_fsync

nop_getattr

nop_inactive

nop_ioctl

nop_link

nop_mkdir

nop_mknod

nop_mmap

nop_offtoblk

nop_open

nop_pagein

nop_pageout

nop_pathconf

nop_read

nop_readdir

nop_readdirattr

nop_readlink

nop_reclaim

nop_remove

nop_rename

nop_revoke

nop_rmdir

nop_searchfs

nop_select

nop_setattr

nop_strategy

nop_symlink

nop_whiteout

nop_write

err_access

err_advlock

err_allocate

err_blktooff

err_blockmap

err_bwrite

err_close

err_copyfile

err_create

err_exchange

err_fsync

err_getattr

err_inactive

err_ioctl

err_link

err_mkdir

err_mknod

err_mmap

err_offtoblk

err_open

err_pagein

err_pageout

err_pathconf

err_read

err_readdir

err_readdirattr

err_readlink

err_reclaim

err_remove

err_rename

err_revoke

err_rmdir

err_searchfs

err_select

err_setattr

err_strategy

err_symlink

err_whiteout

err_write

advisory_read

advisory_read_ext

VNOP_BWRITE

Write a buffer to backing store.

VNOP_FSYNC

Call down to a filesystem to synchronize a file with on-disk state.

VNOP_GETXATTR

Get extended file attributes.

VNOP_IOCTL

Call down to a filesystem or device driver to execute various control operations on or request data about a file.

VNOP_READ

Call down to a filesystem to read file data.

VNOP_SETXATTR

Set extended file attributes.

VNOP_STRATEGY

Initiate I/O on a file (both read and write).

VNOP_WRITE

Call down to the filesystem to write file data.

cache_lookup

Check for a filename in a directory using the VFS name cache.

cache_purge

Remove all data relating to a vnode from the namecache.

cache_purge_negatives

Remove all negative cache entries which are children of a given vnode.

