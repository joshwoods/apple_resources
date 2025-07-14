

- Kernel
- IOKit Fundamentals
- Locks
-  IORecursiveLockUnlock 

Function

# IORecursiveLockUnlock

Unlock a recursive lock.

DriverKitKernelDriverKit 24.4+macOS 10.0+

**DriverKit**

``` source
void IORecursiveLockUnlock(struct IORecursiveLock *lock);
```

**macOS**

``` source
void IORecursiveLockUnlock(IORecursiveLock *lock);
```

## Parameters 

`lock`  

Pointer to the allocated lock.

## Discussion

Undo one call to IORecursiveLockLock, if the lock is now unlocked wake any blocked waiters. Results are undefined if the caller does not balance calls to IORecursiveLockLock with IORecursiveLockUnlock. This function may block and so should not be called from interrupt level or while a spin lock is held.

## See Also

### Recursive Locks

IORecursiveLockAlloc

Allocates and initializes an recursive lock.

IORecursiveLockFree

Frees a recursive lock.

IORecursiveLockGetMachLock

Accessor to a Mach mutex.

IORecursiveLockHaveLock

Check if a recursive lock is held by the calling thread.

IORecursiveLockLock

Lock a recursive lock.

IORecursiveLockSleep

IORecursiveLockSleepDeadline

IORecursiveLockTryLock

Attempt to lock a recursive lock.

IORecursiveLockWakeup

