

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockDestroy 

Function

# IOSimpleLockDestroy

macOS 10.15+

``` source
void IOSimpleLockDestroy(IOSimpleLock *lock);
```

## See Also

### Simple Locks

IOSimpleLockAlloc

Allocates and initializes a spin lock.

IOSimpleLockInit

Initialize a spin lock.

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

