

- Kernel
- IOKit Fundamentals
- Locks
-  IORWLockAlloc 

Function

# IORWLockAlloc

Allocates and initializes a read/write lock.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
struct IORWLock * IORWLockAlloc(void);
```

**macOS**

``` source
IORWLock * IORWLockAlloc(void);
```

## Return Value

Pointer to the allocated lock, or zero on failure.

## Discussion

Allocates and initializes a read/write lock in general purpose memory. Read/write locks provide for multiple readers, one exclusive writer, and are supplied by libkern/locks.h. This function may block and so should not be called from interrupt level or while a spin lock is held. IORWLocks use the global IOKit lock group, IOLockGroup. To simplify kext debugging and lock-heat analysis, consider using lck\_\* locks with a per-driver lock group, as defined in kern/locks.h.

## See Also

### Read/Write Locks

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

IOReadLock

