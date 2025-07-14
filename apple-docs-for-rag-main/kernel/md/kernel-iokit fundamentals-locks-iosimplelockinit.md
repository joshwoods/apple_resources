

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockInit 

Function

# IOSimpleLockInit

Initialize a spin lock.

macOS 10.0+

``` source
void IOSimpleLockInit(IOSimpleLock *lock);
```

## Parameters 

`lock`  

Pointer to the lock.

## Discussion

Initialize an embedded spin lock, to the unlocked state.

## See Also

### Simple Locks

IOSimpleLockAlloc

Allocates and initializes a spin lock.

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

IOSimpleLockUnlock

Unlock a spin lock.

IOSimpleLockUnlockEnableInterrupt

Unlock a spin lock, and restore interrupt state.

