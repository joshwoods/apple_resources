

- Kernel
- sys
- vnop_readlink_args
-  alist 

# alist

Which attributes are wanted for each directory entry.

## See Also

### Fields

vp

Directory in which to enumerate entries' attributes.

uio

Destination information for resulting attributes.

maxcount

Maximum count of files to get attributes for.

options

FSOPT_NOFOLLOW: do not follow symbolic links. FSOPT_NOINMEMUPDATE: do not use data which have been updated since an inode was loaded into memory.

newstate

The "newstate" should be set to a value which changes if the contents of a directory change through an addition or deletion but stays the same otherwise.

eofflag

Should be set to 1 if the end of the directory has been reached.

actualcount

Should be set to number of files whose attributes were written into buffer.

ctx

Context to authenticate for readdirattr request.

