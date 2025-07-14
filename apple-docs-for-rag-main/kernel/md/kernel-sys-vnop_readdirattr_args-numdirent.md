

- Kernel
- sys
- vnop_readdirattr_args
-  numdirent 

# numdirent

Should be set to number of entries written into buffer.

## See Also

### Fields

vp

Directory to enumerate.

uio

Destination information for resulting direntries.

flags

VNODE_READDIR_EXTENDED, VNODE_READDIR_REQSEEKOFF, VNODE_READDIR_SEEKOFF32: Apple-internal flags.

eofflag

Should be set to 1 if the end of the directory has been reached.

ctx

Context to authenticate for readdir request.

