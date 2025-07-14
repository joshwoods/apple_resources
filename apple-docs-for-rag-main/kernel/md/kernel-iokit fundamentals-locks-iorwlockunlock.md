

- Kernel
- IOKit Fundamentals
- Locks
-  IORWLockUnlock 

Function

# IORWLockUnlock

Unlock a read/write lock.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IORWLockUnlock(struct IORWLock *lock);
```

**macOS**

``` source
void IORWLockUnlock(IORWLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Undo one call to IORWLockRead or IORWLockWrite. Results are undefined if the caller has not locked the lock. This function may block and so should not be called from interrupt level or while a spin lock is held.

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

IORWLockWrite

Lock a read/write lock for write.

IORWUnlock

IOWriteLock

IOReadLock

