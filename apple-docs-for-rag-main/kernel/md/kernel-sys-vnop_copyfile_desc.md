

- Kernel
- sys
-  vnop_copyfile_desc 

Global Variable

# vnop_copyfile_desc

macOS 10.4+

``` source
struct vnodeop_desc vnop_copyfile_desc;
```

## See Also

### vnode

vnop_access_desc

vnop_advlock_desc

vnop_allocate_desc

vnop_blktooff_desc

vnop_blockmap_desc

vnop_bwrite_desc

vnop_clonefile_desc

vnop_close_desc

vnop_create_desc

vnop_default_desc

vnop_exchange_desc

vnop_fsync_desc

vnop_getattr_desc

vnop_getattrlistbulk_desc

vnop_getxattr_desc

Write data from a mapped file back to disk.

vnop_inactive_desc

vnop_ioctl_desc

vnop_kqfilt_add_desc

vnop_kqfilt_remove_desc

vnop_link_desc

vnop_listxattr_desc

Remove extended file attributes.

vnop_lookup_desc

vnop_mkdir_desc

vnop_mknod_desc

vnop_mmap_check_desc

vnop_mmap_desc

vnop_mnomap_desc

vnop_offtoblk_desc

vnop_open_desc

vnop_pagein_desc

vnop_pageout_desc

vnop_pathconf_desc

vnop_print_desc

vnop_read_desc

vnop_readdir_desc

vnop_readdirattr_desc

vnop_readlink_desc

vnop_reclaim_desc

vnop_remove_desc

vnop_removexattr_desc

vnop_rename_desc

vnop_renamex_desc

vnop_revoke_desc

vnop_rmdir_desc

vnop_searchfs_desc

vnop_select_desc

vnop_setattr_desc

vnop_setlabel_desc

vnop_setxattr_desc

vnop_strategy_desc

vnop_symlink_desc

vnop_truncate_desc

vnop_whiteout_desc

vnop_write_desc

vnode_addfsref

Mark a vnode as being stored in a filesystem hash.

vnode_authattr

Given a vnode_attr structure, determine what kauth-style actions must be authorized in order to set those attributes.

vnode_authattr_new

Initialize and validate file creation parameters with respect to the current context.

vnode_authorize

Authorize a kauth-style action on a vnode.

vnode_clearautocandidate

vnode_cleardirty

vnode_clearfastdevicecandidate

vnode_clearfsnode

Sets a vnode's filesystem-specific data to be NULL.

vnode_clearmountedon

Clear flags indicating that a block device vnode has been mounted as a filesystem.

vnode_clearnocache

Clear the flag on a vnode indicating that data should not be cached in memory (i.e. we write-through to disk and always read from disk).

vnode_clearnoreadahead

Clear the flag indicating that a vnode should not have data speculatively read in.

vnode_close

Close a file as opened with vnode_open().

vnode_create

Create and initialize a vnode.

vnode_fsnode

Gets the filesystem-specific data associated with a vnode.

vnode_get

Increase the iocount on a vnode.

vnode_get_va_fsid

vnode_getattr

Get vnode attributes.

vnode_getbackingvnode

vnode_getname

Get the name of a vnode from the VFS namecache.

vnode_getparent

Get an iocount on the parent of a vnode.

vnode_getwithref

Increase the iocount on a vnode on which a usecount (persistent reference) is held.

vnode_getwithvid

Increase the iocount on a vnode, checking that the vnode is alive and has not changed vid (i.e. been recycled)

vnode_hascleanblks

Check if a vnode has clean buffers associated with it.

vnode_hasdirtyblks

Check if a vnode has dirty data waiting to be written to disk.

vnode_isautocandidate

vnode_isblk

Determine if a vnode is a block device special file.

vnode_ischr

Determine if a vnode is a character device special file.

vnode_isdir

Determine if a vnode is a directory.

vnode_isdirty

vnode_isfastdevicecandidate

vnode_isfifo

Determine if a vnode is a named pipe.

vnode_isinuse

Determine if the number of persistent (usecount) references on a vnode is greater than a given count.

vnode_islnk

Determine if a vnode is a symbolic link.

vnode_ismount

Determine if there is currently a mount occurring which will cover this vnode.

vnode_ismountedon

Determine if a vnode is a block device on which a filesystem has been mounted.

vnode_isnamedstream

Determine if a vnode is a named stream.

vnode_isnocache

Check if a vnode is set to not have its data cached in memory (i.e. we write-through to disk and always read from disk).

vnode_isnoreadahead

Check if a vnode is set to not have data speculatively read in in hopes of future cache hits.

vnode_isonexternalstorage

vnode_israge

Check if a vnode is marked for rapid aging

vnode_isrecycled

Check if a vnode is dead or in the process of being killed (recycled).

vnode_isreg

Determine if a vnode is a regular file.

vnode_isswap

Determine if a vnode is being used as a swap file.

vnode_issystem

Determine if a vnode is marked as a System vnode.

vnode_isvroot

Determine if a vnode is the root of its filesystem.

vnode_iterate

Perform an operation on (almost) all vnodes from a given mountpoint.

vnode_lookup

Convert a path into a vnode.

vnode_mount

Get the mount structure for the filesystem that a vnode belongs to.

vnode_mountedhere

Returns a pointer to a mount placed on top of a vnode, should it exist.

vnode_needssnapshots

Check if a vnode needs snapshots events (regardless of its ctime status)

vnode_notify

vnode_open

Open a file identified by a path--roughly speaking an in-kernel open(2).

vnode_put

Decrement the iocount on a vnode.

vnode_putname

Release a reference on a name from the VFS cache.

vnode_recycle

Cause a vnode to be reclaimed and prepared for reuse.

vnode_ref

Increment the usecount on a vnode.

vnode_rele

Decrement the usecount on a vnode.

vnode_removefsref

Mark a vnode as no longer being stored in a filesystem hash.

vnode_setattr

Set vnode attributes.

vnode_setautocandidate

vnode_setdirty

vnode_setfastdevicecandidate

vnode_setmountedon

Set flags indicating that a block device vnode has been mounted as a filesystem.

vnode_setmultipath

Mark a vnode as being reachable by multiple paths, i.e. as a hard link.

vnode_setnocache

Set a vnode to not have its data cached in memory (i.e. we write-through to disk and always read from disk).

vnode_setnoreadahead

Set a vnode to not have data speculatively read in in hopes of hitting in cache.

vnode_settag

Set a vnode filesystem-specific "tag."

vnode_specrdev

Return the device id of the device associated with a special file.

vnode_startwrite

vnode_tag

Get the vnode filesystem-specific "tag."

vnode_uncache_credentials

Clear out cached credentials on a vnode.

vnode_update_identity

Update vnode data associated with the vfs cache.

vnode_vfs64bitready

Determine if the filesystem to which a vnode belongs is marked as ready to interact with 64-bit user processes.

vnode_vfsisrdonly

Determine if the filesystem to which a vnode belongs is mounted read-only.

vnode_vfsmaxsymlen

Determine the maximum length of a symbolic link for the filesystem on which a vnode resides.

vnode_vfsname

Get the name of the filesystem to which a vnode belongs.

vnode_vfstypenum

Get the "type number" of the filesystem to which a vnode belongs.

vnode_vid

Return a vnode's vid (generation number), which is constant from creation until reclaim.

vnode_vtype

Return a vnode's type.

vnode_waitforwrites

Wait for the number of pending writes on a vnode to drop below a target.

vnode_writedone

Decrement the count of pending writes on a vnode .

vnode_attr

vnode_fsparam

vnode_t

vnodeopv_desc

vnodeopv_entry_desc

vnop_access_args

Call down to a filesystem to close a file.

vnop_advlock_args

Query a filesystem for path properties.

vnop_allocate_args

Aquire or release and advisory lock on a vnode.

vnop_blktooff_args

List extended attribute keys.

vnop_blockmap_args

Call down to a filesystem to convert a file offset to a logical block number.

vnop_bwrite_args

vnop_clonefile_args

vnop_close_args

Call down to a filesystem to open a file.

vnop_copyfile_args

Write data from a mapped file back to disk.

vnop_create_args

Call down to a filesystem to look for a directory entry by name.

vnop_exchange_args

Call down to a filesystem or device to check if a file is ready for I/O and request later notification if it is not currently ready.

vnop_fsync_args

Inform a filesystem that a file is no longer mapped.

vnop_generic_args

vnop_getattr_args

Call down to a filesystem to see if a kauth-style operation is permitted.

vnop_getattrlistbulk_args

vnop_getxattr_args

Write data from a mapped file back to disk.

vnop_inactive_args

Call down to a filesystem to get the pathname represented by a symbolic link.

vnop_ioctl_args

vnop_kqfilt_add_args

vnop_kqfilt_remove_args

vnop_link_args

Call down to a filesystem to delete a file.

vnop_listxattr_args

Remove extended file attributes.

vnop_lookup_args

vnop_mkdir_args

Call down to a filesystem to rename a file.

vnop_mknod_args

Call down to a filesystem to create a whiteout.

vnop_mmap_args

Call down to a filesystem to invalidate all open file descriptors for a vnode.

vnop_mmap_check_args

vnop_mnomap_args

Notify a filesystem that a file is being mmap-ed.

vnop_offtoblk_args

Call down to a filesystem to convert a logical block number to a file offset.

vnop_open_args

Call down to a filesystem to create a special file.

vnop_pagein_args

Pre-allocate space for a file.

vnop_pageout_args

Pull file data into memory.

vnop_pathconf_args

Release filesystem-internal resources for a vnode.

vnop_read_args

Call down to a filesystem to set vnode attributes.

vnop_readdir_args

Call down to a filesystem to create a symbolic link.

vnop_readdirattr_args

Call down to a filesystem to enumerate directory entries.

vnop_readlink_args

Call down to get file attributes for many files in a directory at once.

vnop_reclaim_args

Notify a filesystem that the last usecount (persistent reference) on a vnode has been dropped.

vnop_remove_args

vnop_removexattr_args

vnop_rename_args

Call down to a filesystem to create a hardlink to a file.

vnop_renamex_args

vnop_revoke_args

Call down to a filesystem to atomically exchange the data of two files.

vnop_rmdir_args

Call down to a filesystem to create a directory.

vnop_searchfs_args

Write data from a mapped file back to disk.

vnop_select_args

vnop_setattr_args

Call down to a filesystem to get vnode attributes.

vnop_setlabel_args

vnop_setxattr_args

vnop_strategy_args

Call down to a filesystem to get information about the on-disk layout of a file region.

vnop_symlink_args

Call down to a filesystem to delete a directory.

vnop_whiteout_args

Call down to a filesystem to create a regular file (VREG).

vnop_write_args

