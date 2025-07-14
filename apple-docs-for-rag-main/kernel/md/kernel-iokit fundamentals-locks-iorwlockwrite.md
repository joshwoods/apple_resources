

- Kernel
- IOKit Fundamentals
- Locks
-  IORWLockWrite 

Function

# IORWLockWrite

Lock a read/write lock for write.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IORWLockWrite(struct IORWLock *lock);
```

**macOS**

``` source
void IORWLockWrite(IORWLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Lock the lock for write, allowing one writer exlusive access. If the lock is held for read or write, block waiting for its unlock. This function may block and so should not be called from interrupt level or while a spin lock is held. Locking the lock recursively from one thread, for read or write, can result in deadlock.

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

IORWUnlock

IOWriteLock

IOReadLock

