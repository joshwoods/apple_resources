

- Kernel
- sys
- vnop_whiteout_args
-  cnp 

# cnp

Description of filename to create.

## See Also

### Fields

dvp

Directory in which to create file.

vpp

Destination for vnode for newly created file.

vap

File creation properties, as seen in vnode_getattr(). Manipulated with VATTR_ISACTIVE, VATTR_RETURN, VATTR_SET_SUPPORTED, and so forth.

ctx

Context against which to authenticate file creation.

