

- Kernel
- IOKit Fundamentals
- Locks
-  IOSimpleLockTryLock 

Function

# IOSimpleLockTryLock

Attempt to lock a spin lock.

macOS 10.0+

``` source
boolean_t IOSimpleLockTryLock(IOSimpleLock *lock);
```

## Parameters 

`lock`  

Pointer to the lock.

## Discussion

Lock the spin lock if it is currently unlocked, and return true. If the lock is held, return false. Successful calls to IOSimpleLockTryLock should be balanced with calls to IOSimpleLockUnlock.

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

IOSimpleLockUnlock

Unlock a spin lock.

IOSimpleLockUnlockEnableInterrupt

Unlock a spin lock, and restore interrupt state.

