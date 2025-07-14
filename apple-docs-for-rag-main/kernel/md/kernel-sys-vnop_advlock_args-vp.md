

- Kernel
- sys
- vnop_advlock_args
-  vp 

# vp

The vnode whose filesystem to query.

## See Also

### Fields

name

Which property to request: see unistd.h. For example: \_PC_CASE_SENSITIVE (is a filesystem case-sensitive?). Only one property can be requested at a time.

retval

Destination for value of property.

ctx

Context to authenticate for pathconf request.

