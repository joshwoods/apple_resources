

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockAlloc 

Function

# IOSimpleLockAlloc

Allocates and initializes a spin lock.

macOS 10.0+

``` source
IOSimpleLock * IOSimpleLockAlloc(void);
```

## Return Value

Pointer to the allocated lock, or zero on failure.

## Discussion

Allocates and initializes a spin lock in general purpose memory. Spin locks provide non-blocking mutual exclusion for synchronization between thread context and interrupt context, or for multiprocessor synchronization, and are supplied by libkern/locks.h. This function may block and so should not be called from interrupt level or while a spin lock is held. IOSimpleLocks use the global IOKit lock group, IOLockGroup. To simplify kext debugging and lock-heat analysis, consider using lck\_\* locks with a per-driver lock group, as defined in kern/locks.h.

## See Also

### Simple Locks

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

IOSimpleLockUnlockEnableInterrupt

Unlock a spin lock, and restore interrupt state.

