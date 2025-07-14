

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockFree 

Function

# IOSimpleLockFree

Frees a spin lock.

macOS 10.0+

``` source
void IOSimpleLockFree(IOSimpleLock *lock);
```

## Parameters 

`lock`  

Pointer to the lock.

## Discussion

Frees a lock allocated with IOSimpleLockAlloc.

## See Also

### Simple Locks

IOSimpleLockAlloc

Allocates and initializes a spin lock.

IOSimpleLockInit

Initialize a spin lock.

IOSimpleLockDestroy

IOSimpleLockGetMachLock

Accessor to a Mach spin lock.

IOSimpleLockLock

Lock a spin lock.

IOSimpleLockLockDisableInterrupt

Lock a spin lock.

IOSimpleLockTryLock

Attempt to lock a spin lock.

IOSimpleLockUnlock

Unlock a spin lock.

IOSimpleLockUnlockEnableInterrupt

Unlock a spin lock, and restore interrupt state.

