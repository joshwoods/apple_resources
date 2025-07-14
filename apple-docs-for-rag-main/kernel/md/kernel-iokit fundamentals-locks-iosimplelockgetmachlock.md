

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockGetMachLock 

Function

# IOSimpleLockGetMachLock

Accessor to a Mach spin lock.

macOS 10.4+

``` source
lck_spin_t * IOSimpleLockGetMachLock(IOSimpleLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Accessor to the Mach spin lock.

## See Also

### Simple Locks

IOSimpleLockAlloc

Allocates and initializes a spin lock.

IOSimpleLockInit

Initialize a spin lock.

IOSimpleLockDestroy

IOSimpleLockFree

Frees a spin lock.

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

