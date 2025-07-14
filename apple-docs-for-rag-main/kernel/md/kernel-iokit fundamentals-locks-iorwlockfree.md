

- Kernel
- IOKit Fundamentals
- Locks
-  IORWLockFree 

Function

# IORWLockFree

Frees a read/write lock.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IORWLockFree(struct IORWLock *lock);
```

**macOS**

``` source
void IORWLockFree(IORWLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Frees a lock allocated with IORWLockAlloc. Lock should be unlocked with no waiters.

## See Also

### Read/Write Locks

IORWLockAlloc

Allocates and initializes a read/write lock.

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

