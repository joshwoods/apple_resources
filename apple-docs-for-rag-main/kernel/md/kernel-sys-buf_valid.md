

- Kernel
- sys
-  buf_valid 

Function

# buf_valid

Check if a buffer contains valid data.

macOS 10.4+

``` source
int buf_valid(buf_t bp);
```

## Parameters 

`bp`  

Buffer to test.

## Return Value

Nonzero if buffer has valid data, 0 if not.

## See Also

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

buf_vnode

Get the vnode associated with a buffer.

buf_wcred

Get the credential associated with a buffer for writing.

bufattr_ioscheduled

bufattr_markioscheduled

