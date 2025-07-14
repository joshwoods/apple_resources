

- Kernel
-  vfs 

API Collection

# vfs

Access the virtual file-system interfaces.

## Topics

### Functions

vflush

Reclaim the vnodes for a mount.

vfs_64bitready

Check if the filesystem associated with a mountpoint is marked ready for interaction with 64-bit user processes.

vfs_addname

Deprecated

vfs_attr_pack

vfs_attr_pack_ext

vfs_authcache_ttl

Determine the time-to-live of cached authorized credentials for files in this filesystem.

vfs_authopaque

Determine if a filesystem's authorization decisions occur remotely.

vfs_authopaqueaccess

Check if a filesystem is marked as having reliable remote VNOP_ACCESS support.

vfs_busy

"Busy" a mountpoint.

vfs_clearauthcache_ttl

Remove time-to-live controls for cached credentials on a filesytem. Filesystems with remote authorization decisions (opaque) will still have KAUTH_VNODE_SEARCH rights cached for a default of CACHED_LOOKUP_RIGHT_TTL seconds.

vfs_clearauthopaque

vfs_clearauthopaqueaccess

Mark a filesystem as not having remote VNOP_ACCESS support.

vfs_clearextendedsecurity

Mark a filesystem as NOT supporting security controls beyond POSIX permissions.

vfs_clearflags

Clear flags on a mount.

vfs_context_create

Create a new vfs_context_t with appropriate references held.

vfs_context_current

Get the vfs_context for the current thread, or the kernel context if there is no context for current thread.

vfs_context_get_special_port

vfs_context_is64bit

Determine if a vfs_context_t corresponds to a 64-bit user process.

vfs_context_issignal

Get a bitfield of pending signals for the BSD process associated with a vfs_context_t.

vfs_context_pid

Get the process id of the BSD process associated with a vfs_context_t.

vfs_context_proc

Get the BSD process structure associated with a vfs_context_t.

vfs_context_rele

Release references on components of a context and deallocate it.

vfs_context_set_special_port

vfs_context_suser

Determine if a vfs_context_t corresponds to the superuser.

vfs_context_ucred

Get the credential associated with a vfs_context_t.

vfs_devblocksize

Get the block size of the device underlying a mount.

vfs_event_init

This function should not be called by kexts.

vfs_event_signal

Post a kqueue-style event on a filesystem (EVFILT_FS).

vfs_flags

Retrieve mount flags.

vfs_fsadd

Register a filesystem with VFS.

vfs_fsprivate

Get filesystem-private mount data.

vfs_fsremove

Unregister a filesystem with VFS.

vfs_get_notify_attributes

vfs_getnewfsid

Generate a unique filesystem ID for a mount and store it in the mount structure.

vfs_getvfs

Given a filesystem ID, look up a mount structure.

vfs_init_io_attributes

Set I/O attributes on a mountpoint based on device properties.

vfs_ioattr

Get I/O attributes associated with a mounpoint.

vfs_isforce

Determine if a forced unmount is in progress.

vfs_isrdonly

Determine if a filesystem is mounted read-only.

vfs_isrdwr

Determine if a filesystem is mounted with writes enabled.

vfs_isreload

Determine if a reload of filesystem data is in progress. This can only be the case for a read-only filesystem; all data is brought in from secondary storage.

vfs_issynchronous

Determine if writes to a filesystem occur synchronously.

vfs_isunmount

Determine if an unmount is in progress.

vfs_isupdate

Determine if a mount update is in progress.

vfs_iswriteupgrade

Determine if a filesystem is mounted read-only but a request has been made to upgrade to read-write.

vfs_iterate

Iterate over all mountpoints with a callback. Used, for example, by sync().

vfs_maxsymlen

Get the maximum length of a symbolic link on a filesystem.

vfs_mountedon

Check whether a given block device has a filesystem mounted on it.

vfs_name

Copy filesystem name into a buffer.

vfs_nspace_server

vfs_nspace_server_routine

vfs_removename

Deprecated

vfs_rootvnode

Returns the root vnode with an iocount.

vfs_set_root_unmounted_cleanly

vfs_setauthcache_ttl

Enable credential caching and set time-to-live of cached authorized credentials for files in this filesystem.

vfs_setauthopaque

Mark a filesystem as having authorization decisions controlled remotely.

vfs_setauthopaqueaccess

Mark a filesystem as having remote VNOP_ACCESS support.

vfs_setextendedsecurity

Mark a filesystem as supporting security controls beyond POSIX permissions.

vfs_setflags

Set flags on a mount.

vfs_setfsprivate

Set filesystem-private mount data.

vfs_setioattr

Set I/O attributes associated with a mounpoint.

vfs_setlocklocal

Mark a filesystem as using VFS-level advisory locking support.

vfs_setmaxsymlen

Set the maximum length of a symbolic link on a filesystem.

vfs_setup_vattr_from_attrlist

vfs_statfs

Get information about filesystem status.

vfs_typenum

Get (archaic) filesystem type number.

vfs_unbusy

"Unbusy" a mountpoint by releasing its read-write lock.

vfs_unmountbyfsid

Find a filesystem by ID and unmount it.

vfs_update_vfsstat

Update cached filesystem status information in the VFS mount structure.

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

cache_enter

Add a (name,vnode) entry to the VFS namecache.

cache_lookup

Check for a filename in a directory using the VFS name cache.

cache_purge

Remove all data relating to a vnode from the namecache.

cache_purge_negatives

Remove all negative cache entries which are children of a given vnode.

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

sys

Access general system utilities for time, file systems, and system information.

vm

Interact with the virtual memory system.

