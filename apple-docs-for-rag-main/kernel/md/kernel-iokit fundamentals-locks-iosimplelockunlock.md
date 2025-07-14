

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockUnlock 

Function

# IOSimpleLockUnlock

Unlock a spin lock.

macOS 10.0+

``` source
void IOSimpleLockUnlock(IOSimpleLock *lock);
```

## Parameters 

`lock`  

Pointer to the lock.

## Discussion

Unlock the lock, and restore preemption. Results are undefined if the caller has not locked the lock.

## See Also

### Simple Locks

IOSimpleLockAlloc

Allocates and initializes a spin lock.

IOSimpleLockInit

Initialize a spin lock.

IOSimpleLockDestroy

IOSimpleLockFree

Frees a spin lock.

IOSimpleLockGetMachLock

Accessor to a Mach spin lock.

IOSimpleLockLock

Lock a spin lock.

IOSimpleLockLockDisableInterrupt

Lock a spin lock.

IOSimpleLockTryLock

Attempt to lock a spin lock.

IOSimpleLockUnlockEnableInterrupt

Unlock a spin lock, and restore interrupt state.

