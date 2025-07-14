

- Kernel
- IOKit Fundamentals
- Locks
-  IORWLockRead 

Function

# IORWLockRead

Lock a read/write lock for read.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IORWLockRead(struct IORWLock *lock);
```

**macOS**

``` source
void IORWLockRead(IORWLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Lock the lock for read, allowing multiple readers when there are no writers. If the lock is held for write, block waiting for its unlock. This function may block and so should not be called from interrupt level or while a spin lock is held. Locking the lock recursively from one thread, for read or write, can result in deadlock.

## See Also

### Read/Write Locks

IORWLockAlloc

Allocates and initializes a read/write lock.

IORWLockFree

Frees a read/write lock.

IORWLockGetMachLock

Accessor to a Mach read/write lock.

IORWLockUnlock

Unlock a read/write lock.

IORWLockWrite

Lock a read/write lock for write.

IORWUnlock

IOWriteLock

IOReadLock

