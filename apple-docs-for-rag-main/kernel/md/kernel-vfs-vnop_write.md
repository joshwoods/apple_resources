

- Kernel
- vfs
-  VNOP_WRITE 

Function

# VNOP_WRITE

Call down to the filesystem to write file data.

macOS 10.4+

``` source
errno_t VNOP_WRITE(vnode_t vp, struct uio *uio, int ioflag, vfs_context_t ctx);
```

## Parameters 

`vp`  

The vnode to write to.

`uio`  

Description of request, including file offset, amount of data to write, source address for data, and whether that destination is in kernel or user space.

`ctx`  

Context against which to authenticate write request.

## Return Value

0 for success or a filesystem-specific error. VNOP_WRITE() can return success even if less data was written than originally requested; returning an error value should indicate that something actually went wrong.

## Discussion

VNOP_WRITE() is to write() as VNOP_READ() is to read(). The filesystem may use the buffer cache, the cluster layer, or an alternative method to write its data; uio routines will be used to see that data is copied to the correct virtual address in the correct address space and will update its uio argument to indicate how much data has been moved.

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

cache_enter

Add a (name,vnode) entry to the VFS namecache.

cache_lookup

Check for a filename in a directory using the VFS name cache.

cache_purge

Remove all data relating to a vnode from the namecache.

cache_purge_negatives

Remove all negative cache entries which are children of a given vnode.

