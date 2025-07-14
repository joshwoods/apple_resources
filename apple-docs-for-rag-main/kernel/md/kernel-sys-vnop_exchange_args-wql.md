

- Kernel
- sys
- vnop_exchange_args
-  wql 

# wql

Opaque object to pass to selrecord().

## See Also

### Fields

vp

The vnode to check for I/O readiness.

which

What kind of I/O is desired: FREAD, FWRITE.

fflags

Flags from fileglob as seen in fcntl.h, e.g. O_NONBLOCK, O_APPEND.

ctx

Context to authenticate for select request.

