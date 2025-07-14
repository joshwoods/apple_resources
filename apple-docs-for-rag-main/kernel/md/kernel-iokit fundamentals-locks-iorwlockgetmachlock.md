

- Kernel
- IOKit Fundamentals
- Locks
-  IORWLockGetMachLock 

Function

# IORWLockGetMachLock

Accessor to a Mach read/write lock.

macOS 10.4+

``` source
lck_rw_t * IORWLockGetMachLock(IORWLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Accessor to the Mach read/write lock.

## See Also

### Read/Write Locks

IORWLockAlloc

Allocates and initializes a read/write lock.

IORWLockFree

Frees a read/write lock.

IORWLockRead

Lock a read/write lock for read.

IORWLockUnlock

Unlock a read/write lock.

IORWLockWrite

Lock a read/write lock for write.

IORWUnlock

IOWriteLock

IOReadLock

