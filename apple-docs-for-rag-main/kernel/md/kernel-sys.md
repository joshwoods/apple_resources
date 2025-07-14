

- Kernel
-  sys 

API Collection

# sys

Access general system utilities for time, file systems, and system information.

## Topics

### Block Device

bdevsw_add

bdevsw_isfree

bdevsw_remove

cdevsw_add

cdevsw_add_with_bdev

cdevsw_isfree

cdevsw_remove

### Buffers

buf_alloc

Allocate an uninitialized buffer.

buf_attr

Gets the attributes for this buf.

buf_bawrite

Start an asychronous write on a buffer.

buf_bdwrite

Mark a buffer for delayed write.

buf_biodone

Mark an I/O as completed.

buf_biowait

Wait for I/O on a buffer to complete.

buf_blkno

Get physical block number associated with a buffer, in the sense of VNOP_BLOCKMAP.

buf_bread

Synchronously read a block of a file.

buf_breadn

Read a block from a file with read-ahead.

buf_brelse

Release any claim to a buffer, sending it back to free lists.

buf_bwrite

Write a buffer's data to backing store.

buf_callback

Get the function set to be called when I/O on a buffer completes.

buf_clear

Zero out the storage associated with a buffer.

buf_clear_redundancy_flags

Clear flags on a buffer. @discussion: buffer_redundancy_flags &= ~flags

buf_clearflags

Clear flags on a buffer. @discussion: buffer_flags &= ~flags

buf_clone

Clone a buffer with a restricted range and an optional callback.

buf_count

Get count of valid bytes in a buffer. This may be less than the space allocated to the buffer.

buf_create_shadow

Create a shadow buffer with optional private storage and an optional callback.

buf_dataptr

Get the address at which a buffer's data is stored; for iobufs, this must be set with buf_setdataptr(). See buf_map().

buf_device

Get the device ID associated with a buffer.

buf_dirtyend

Get the ending offset of the dirty region associated with a buffer.

buf_dirtyoff

Get the starting offset of the dirty region associated with a buffer.

buf_drvdata

Get driver-specific data from a buffer.

buf_error

Get the error value associated with a buffer.

buf_flags

Get flags set on a buffer.

buf_flushdirtyblks

Write dirty file blocks to disk.

buf_free

Free a buffer that was allocated with buf_alloc().

buf_fromcache

Check if a buffer's data was found in core.

buf_fsprivate

Get filesystem-specific data from a buffer.

buf_fua

Check if a buffer is marked for write through disk caches.

buf_getblk

Traditional buffer cache routine to get a buffer corresponding to a logical block in a file.

buf_geteblk

Get a metadata buffer which is marked invalid and not associated with any vnode.

buf_invalblkno

Invalidate a filesystem logical block in a file.

buf_invalidateblks

Invalidate all the blocks associated with a vnode.

buf_iterate

Perform some operation on all buffers associated with a vnode.

buf_lblkno

Get logical block number associated with a buffer.

buf_map

Get virtual mappings for buffer data.

buf_markaged

Mark a buffer as "aged," i.e. as a good candidate to be discarded and reused after buf_brelse().

buf_markclean

buf_markdelayed

Mark a buffer as a delayed write: mark it dirty without actually scheduling I/O.

buf_markeintr

Mark a buffer as having been interrupted during I/O.

buf_markfua

Mark a buffer for write through disk cache, if disk supports it.

buf_markinvalid

Mark a buffer as not having valid data and being ready for immediate reuse after buf_brelse().

buf_markstatic

Mark a buffer as being likely to contain static data.

buf_meta_bread

Synchronously read a metadata block of a file.

buf_meta_breadn

Read a metadata block from a file with read-ahead.

buf_proc

Get the process associated with this buffer.

buf_rcred

Get the credential associated with a buffer for reading.

buf_redundancy_flags

Get redundancy flags set on a buffer.

buf_reset

Reset I/O flag state on a buffer.

buf_resid

Get a count of bytes which were not consumed by an I/O on a buffer.

buf_set_redundancy_flags

Set redundancy flags on a buffer. @discussion: buffer_redundancy_flags \|= flags

buf_setblkno

Set physical block number associated with a buffer.

buf_setcallback

Set a function to be called once when I/O on a buffer completes.

buf_setcount

Set count of valid bytes in a buffer. This may be less than the space allocated to the buffer.

buf_setdataptr

Set the address at which a buffer's data will be stored.

buf_setdevice

Set the device associated with a buffer.

buf_setdirtyend

Set the ending offset of the dirty region associated with a buffer.

buf_setdirtyoff

Set the starting offset of the dirty region associated with a buffer.

buf_setdrvdata

Set driver-specific data on a buffer.

buf_seterror

Set an error value on a buffer.

buf_setflags

Set flags on a buffer. @discussion: buffer_flags \|= flags

buf_setfsprivate

Set filesystem-specific data on a buffer.

buf_setlblkno

Set logical block number associated with a buffer.

buf_setresid

Set a count of bytes outstanding for I/O in a buffer.

buf_setsize

Set size of data region allocated to a buffer.

buf_setupl

Set the UPL (Universal Page List), and offset therein, on a buffer.

buf_setvnode

Set the vnode associated with a buffer.

buf_shadow

returns true if 'bp' is a shadow of another buffer.

buf_size

Get size of data region allocated to a buffer.

buf_static

Check if a buffer contains static data.

buf_strategy

Pass an I/O request for a buffer down to the device layer.

buf_unmap

Release mappings for buffer data.

buf_upl

Get the upl (Universal Page List) associated with a buffer.

buf_uploffset

Get the offset into a UPL at which this buffer begins.

buf_valid

Check if a buffer contains valid data.

buf_vnode

Get the vnode associated with a buffer.

buf_wcred

Get the credential associated with a buffer for writing.

bufattr_ioscheduled

bufattr_markioscheduled

### General

bsd_timeout

bsd_untimeout

### Serialization

OSUnserialize

OSUnserializeBinary

OSUnserializeXML

### control

ctl_deregister

ctl_enqueuedata

ctl_enqueuembuf

ctl_getenqueuereadable

ctl_getenqueuespace

ctl_register

### file

file_drop

file_flags

file_socket

file_vnode

file_vnode_withvid

### proc

proc_best_name

proc_chrooted

proc_csflags

proc_exiting

proc_find

proc_forcequota

proc_gettty

proc_gettty_dev

proc_in_teardown

proc_is64bit

proc_is64bit_data

proc_is_classic

proc_isinferior

proc_issetugid

proc_issignal

proc_name

proc_noremotehang

proc_original_ppid

proc_pgrpid

Get the process group id for the passed-in process.

proc_pid

proc_platform

proc_ppid

proc_rele

proc_sdk

proc_self

proc_selfcsflags

proc_selfname

proc_selfpgrpid

Get the process group id for the current process, as with proc_pgrpid().

proc_selfpid

proc_selfppid

proc_send_synchronous_EXC_RESOURCE

proc_sessionid

proc_signal

proc_suser

proc_tbe

proc_ucredDeprecated

current_proc

current_proc_EXTERNAL

### sysctl

sysctl_handle_int

sysctl_handle_int2quad

sysctl_handle_long

sysctl_handle_opaque

sysctl_handle_quad

sysctl_handle_string

sysctl_io_number

sysctl_io_opaque

sysctl_io_string

sysctl_register_oid

sysctl_unregister_oid

sysctlbyname

Gets or sets information about the system and environment.

sysctl__children

sysctl__debug_children

sysctl__hw_children

sysctl__kern_children

sysctl__machdep_children

sysctl__net_children

sysctl__sysctl_children

sysctl__user_children

sysctl__vfs_children

sysctl__vm_children

### throttle

throttle_info_create

throttle_info_disable_throttle

throttle_info_io_will_be_throttled

throttle_info_mount_ref

throttle_info_mount_rel

throttle_info_ref_by_mask

throttle_info_rel_by_mask

throttle_info_release

throttle_info_update

throttle_info_update_by_mask

throttle_lowpri_io

throttle_lowpri_io_will_be_throttled

throttle_set_thread_io_policy

### ubc

ubc_blktooff

ubc_create_upl

ubc_getcred

ubc_getsize

ubc_msync

ubc_offtoblk

ubc_page_op

ubc_pages_resident

ubc_range_op

ubc_setsize

ubc_setthreadcred

ubc_upl_abort

ubc_upl_abort_range

ubc_upl_commit

ubc_upl_commit_range

ubc_upl_map

ubc_upl_maxbufsize

ubc_upl_pageinfo

ubc_upl_range_needed

ubc_upl_unmap

cluster_bp

cluster_bp_ext

cluster_copy_ubc_data

cluster_copy_upl_data

cluster_lock_direct_read

cluster_pagein

cluster_pagein_ext

cluster_pageout

cluster_pageout_ext

cluster_push

cluster_push_err

cluster_push_ext

cluster_read

cluster_read_ext

cluster_unlock_direct_read

cluster_update_state

cluster_write

cluster_write_ext

cluster_zero

### vnode

vnop_access_desc

vnop_advlock_desc

vnop_allocate_desc

vnop_blktooff_desc

vnop_blockmap_desc

vnop_bwrite_desc

vnop_clonefile_desc

vnop_close_desc

vnop_copyfile_desc

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

## See Also

### BSD

architecture

Access machine-level and architectural information about the current platform.

bsm

Audit resource usage on the system.

hfs

Access HFS file-system data structures.

kern

Access kernel-level interfaces including clock, task, kernel extension, lock, and compression utilities.

Math

Perform mathematical operations and manipulate integer, float, and double values.

miscfs

Access device nodes and other file-system entities.

net

Access network-related utilities.

Strings

Compare, convert, and catenate strings and access the resulting content of those strings.

vfs

Access the virtual file-system interfaces.

vm

Interact with the virtual memory system.

