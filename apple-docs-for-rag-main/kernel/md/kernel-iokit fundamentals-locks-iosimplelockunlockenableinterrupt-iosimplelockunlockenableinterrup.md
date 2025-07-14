

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockUnlockEnableInterrupt 

Function

# IOSimpleLockUnlockEnableInterrupt

Unlock a spin lock, and restore interrupt state.

macOS 10.0+

``` source
void IOSimpleLockUnlockEnableInterrupt(IOSimpleLock *lock, IOInterruptState state);
```

## Parameters 

`lock`  

Pointer to the lock.

`state`  

The interrupt state returned by IOSimpleLockLockDisableInterrupt()

## Discussion

Unlock the lock, and restore preemption and interrupts to the state as they were when the lock was taken. Results are undefined if the caller has not locked the lock.

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

IOSimpleLockUnlock

Unlock a spin lock.

