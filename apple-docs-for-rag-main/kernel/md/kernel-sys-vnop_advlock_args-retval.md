

- Kernel
- sys
- vnop_advlock_args
-  retval 

# retval

Destination for value of property.

## See Also

### Fields

vp

The vnode whose filesystem to query.

name

Which property to request: see unistd.h. For example: \_PC_CASE_SENSITIVE (is a filesystem case-sensitive?). Only one property can be requested at a time.

ctx

Context to authenticate for pathconf request.

