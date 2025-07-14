

- Kernel
- vfs
-  VNOP_IOCTL 

Function

# VNOP_IOCTL

Call down to a filesystem or device driver to execute various control operations on or request data about a file.

macOS 10.4+

``` source
errno_t VNOP_IOCTL(vnode_t vp, u_long command, caddr_t data, int fflag, vfs_context_t ctx);
```

## Parameters 

`vp`  

The vnode to execute the command on.

`command`  

Identifier for action to take.

`data`  

Pointer to data; this can be an integer constant (of 32 bits only) or an address to be read from or written to, depending on "command." If it is an address, it is valid and resides in the kernel; callers of VNOP_IOCTL() are responsible for copying to and from userland.

`ctx`  

Context against which to authenticate ioctl request.

## Return Value

0 for success or a filesystem-specific error.

## Discussion

Ioctl controls are typically associated with devices, but they can in fact be passed down for any file; they are used to implement any of a wide range of controls and information requests. fcntl() calls VNOP_IOCTL for several commands, and will attempt a VNOP_IOCTL if it is passed an unknown command, though no copyin or copyout of arguments can occur in this case--the "arg" must be an integer value. Filesystems can define their own fcntls using this mechanism. How ioctl commands are structured is slightly complicated; see the manual page for ioctl(2).

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

VNOP_READ

Call down to a filesystem to read file data.

VNOP_SETXATTR

Set extended file attributes.

VNOP_STRATEGY

Initiate I/O on a file (both read and write).

VNOP_WRITE

Call down to the filesystem to write file data.

cache_enter

Add a (name,vnode) entry to the VFS namecache.

cache_lookup

Check for a filename in a directory using the VFS name cache.

cache_purge

Remove all data relating to a vnode from the namecache.

cache_purge_negatives

Remove all negative cache entries which are children of a given vnode.

