

- Kernel
- sys
- vnop_allocate_args
-  fl 

# fl

Description of file region to lock. l_whence is as with "lseek." Includes a type: F_RDLCK (shared lock), F_UNLCK (unlock) , and F_WRLCK (exclusive lock).

## See Also

### Fields

vp

The vnode to lock or unlock.

id

Identifier for lock holder: ignored by most filesystems.

op

Which locking operation: F_SETLK: set locking information about a region. F_GETLK: get locking information about the specified region. F_UNLCK: Unlock a region.

flags

F_FLOCK: use flock() semantics. F_POSIX: use POSIX semantics. F_WAIT: sleep if necessary. F_PROV: Non-coelesced provisional lock (unused in xnu).

ctx

Context to authenticate for advisory locking request.

timeout

Timespec for timeout in case of F_SETLKWTIMEOUT.

