

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockLock 

Function

# IOSimpleLockLock

Lock a spin lock.

macOS 10.0+

``` source
void IOSimpleLockLock(IOSimpleLock *lock);
```

## Parameters 

`lock`  

Pointer to the lock.

## Discussion

Lock the spin lock. If the lock is held, spin waiting for its unlock. Spin locks disable preemption, cannot be held across any blocking operation, and should be held for very short periods. When used to synchronize between interrupt context and thread context they should be locked with interrupts disabled - IOSimpleLockLockDisableInterrupt() will do both. Locking the lock recursively from one thread will result in deadlock.

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

IOSimpleLockLockDisableInterrupt

Lock a spin lock.

IOSimpleLockTryLock

Attempt to lock a spin lock.

IOSimpleLockUnlock

Unlock a spin lock.

IOSimpleLockUnlockEnableInterrupt

Unlock a spin lock, and restore interrupt state.

