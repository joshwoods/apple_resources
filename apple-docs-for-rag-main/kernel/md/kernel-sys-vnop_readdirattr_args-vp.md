

- Kernel
- sys
- vnop_readdirattr_args
-  vp 

# vp

Directory to enumerate.

## See Also

### Fields

uio

Destination information for resulting direntries.

flags

VNODE_READDIR_EXTENDED, VNODE_READDIR_REQSEEKOFF, VNODE_READDIR_SEEKOFF32: Apple-internal flags.

eofflag

Should be set to 1 if the end of the directory has been reached.

numdirent

Should be set to number of entries written into buffer.

ctx

Context to authenticate for readdir request.

