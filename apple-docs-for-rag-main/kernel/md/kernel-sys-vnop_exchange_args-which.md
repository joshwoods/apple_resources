

- Kernel
- sys
- vnop_exchange_args
-  which 

# which

What kind of I/O is desired: FREAD, FWRITE.

## See Also

### Fields

vp

The vnode to check for I/O readiness.

fflags

Flags from fileglob as seen in fcntl.h, e.g. O_NONBLOCK, O_APPEND.

wql

Opaque object to pass to selrecord().

ctx

Context to authenticate for select request.

