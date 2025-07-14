

- Kernel
- IOKit Fundamentals
- Locks
-  IOReadLock 

Function

# IOReadLock

macOS 10.0+

``` source
void IOReadLock(IORWLock *lock);
```

## See Also

### Read/Write Locks

IORWLockAlloc

Allocates and initializes a read/write lock.

IORWLockFree

Frees a read/write lock.

IORWLockGetMachLock

Accessor to a Mach read/write lock.

IORWLockRead

Lock a read/write lock for read.

IORWLockUnlock

Unlock a read/write lock.

IORWLockWrite

Lock a read/write lock for write.

IORWUnlock

IOWriteLock

