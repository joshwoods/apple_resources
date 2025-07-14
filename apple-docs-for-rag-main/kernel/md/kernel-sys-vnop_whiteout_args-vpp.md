

- Kernel
- sys
- vnop_whiteout_args
-  vpp 

# vpp

Destination for vnode for newly created file.

## See Also

### Fields

dvp

Directory in which to create file.

cnp

Description of filename to create.

vap

File creation properties, as seen in vnode_getattr(). Manipulated with VATTR_ISACTIVE, VATTR_RETURN, VATTR_SET_SUPPORTED, and so forth.

ctx

Context against which to authenticate file creation.

