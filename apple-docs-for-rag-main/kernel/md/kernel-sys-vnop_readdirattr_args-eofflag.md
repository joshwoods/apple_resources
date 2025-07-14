

- Kernel
- sys
- vnop_readdirattr_args
-  eofflag 

# eofflag

Should be set to 1 if the end of the directory has been reached.

## See Also

### Fields

vp

Directory to enumerate.

uio

Destination information for resulting direntries.

flags

VNODE_READDIR_EXTENDED, VNODE_READDIR_REQSEEKOFF, VNODE_READDIR_SEEKOFF32: Apple-internal flags.

numdirent

Should be set to number of entries written into buffer.

ctx

Context to authenticate for readdir request.

